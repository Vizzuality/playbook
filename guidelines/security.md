# Security

## Online accounts

This section covers security around online services:

- Use strong passwords for all services (personal or not). A strong password should be unique (not used in multiple services), at least 15 characters long, and mix upper and lower case characters, numbers and special characters. 
- Enable 2FA for all services for which you have an individual account - your email account, Github, AWS, LastPass, etc
- For non personal services auto-generate 15+ character ascii passwords and store in LastPass. Passwords can and will be modified regularly
- Share passwords in folders, not directly with people, then invite people to folders

LastPass allows you to quickly and easily generate passwords that match the criteria above. It can also warn you in case
 it detects you are sharing the same password across multiple services, which you can use to quickly audit your current
 passwords
 
 
### What to do in case one of your online accounts is compromised
 
If you suspect a personal or non personal account has been compromised or a device (computer, mobile phone, tablet, etc) with open sessions or access to 2FA codes has been lost or stolen please:
 
- Ask your colleagues for help
- Close all open sessions
- Change password for all affected services
- Refer to the documentation of the affected service(s) on how to invalidate your lost 2FA device credentials 


## Sharing passwords

### Internally

When sharing passwords with other team members, do so using LastPass. LastPass entries should be grouped within a LastPass folder, which can then be shared with the project team and ideally also relevant staff from outside of the strict project team, who might be able to step in and help with a project when needed.

### With clients

Each client organisation has different practices around security and password management, making this specific guideline 
less clear. If the client organisation has no specific policy around password management, suggest using LastPass, as it's
a free service anyone can sign up for. 

If the client does not want to adopt LastPass, or already uses another tool for this purpose, use your best judgment on
the best way to share passwords. However you should always keep in mind that the following are NOT safe ways to share
passwords:
- Slack/other chat tools
- Email
- Basecamp
- Hangout/Skype/etc
- Google docs/drive/etc

In certain scenarios, the client will request that we send the password through one of these channels anyway. We should
warn about the security risk of this, and request that the receiving person change that specific password as soon as they
 receive it.

## Internet access

When outside the office/your home, avoid connecting to public wifi networks. There's a [wide range of attacks](http://blog.privatewifi.com/how-wifi-hotspot-hacks-occur/) that can be executed around the concept of wifi hotspots, and even
legitimate hotspots usually track your browsing habits or inject annoying ads into your browser.

As an alternative, you can use a tethered connection from your smartphone to your computer, or use a VPN service when using a public hotspot network.


## Computers

Your computer should have Full Disk Encryption enabled. All modern operating systems support this out of the box 
(Apple calls its implementation FileVault), and the performance impact is negligible or non-existent, depending on
your hardware and OS.

Your login password should be complex enough as to not be guessable through trial-and-errors (avoid relatives names, birth dates, phone numbers, etc).

Be mindful of what devices you connect to your computer. Malware DOES exist for MacOS, and it can be injected into your computer [from where you least expect](https://www.techspot.com/news/75923-british-security-expert-mods-usb-c-apple-charger.html).

## Digital certificates

If you're working or generating digital certificates of any kind - like the ones used by Apple to sign iOS apps, for example - make sure to follow these steps: 

1. Any attached password or username or information required to use it. 
2. What does this certificate have access rights too?
3. Does this certificate have access to NDA material? 
4. Stored in a secure place on LastPass (yes LastPass supports files).
5. If you’re creating a certificate, make sure you're registering it on a company profile, not your own personal credentials. 

If a certificate has to be shared with a client, make sure the certificate does not have access to any other client information than is required. Use the same guidelines as you would use to share a password to share a certificate.

## Other sensitive info

In general, any other types of sensitive info used in projects or services, like secret keys, authorization tokens, etc should be stored and saved through LastPass using the "secure notes" feature. When storing and sharing please include all the relevant info:

- The key ot token itself
- The service/project it is for
- Date of creation (and expiry if appropriate)
- Usage instructions (eg. include on config file)
- Contact person

## Github

If you use git and github, this section is for you. If you don't, move along, here be dragons.

### Transfer protocol

Github supports two main methods of communicating with their servers: SSH or HTTPS. Both are secure, and can be used 
interchangeably. You can find a detailed comparison of these two options (and a few others) [in this link](https://gist.github.com/grawity/4392747).
You should always use one of these two methods, as they are the only ones with security built in. You can find
 Github's recommendation [here](https://help.github.com/articles/which-remote-url-should-i-use/) - this has been known
 to change frequently, so don't worry if you are not using their recommended version. Also keep in mind that they 
 behave in slightly different ways during day-to-day usage, as SSH requires less password management over HTTPS.

### Signing commits

While not required, it's strongly recommended that you sign your commits using a GPG key to protect against 
[commit spoofing](https://medium.com/@pjbgf/spoofing-git-commits-7bef357d72f0). The process is similar to generating SSH
keys, and you can find the instructions to do so [in this link](https://help.github.com/articles/signing-commits-using-gpg/).
Signed commits will display a "Verified" message next to them - you can see an example of this in PR merge commits.

### Deploy keys

In some scenarios, certain Github projects need to be cloned onto servers or other similar environments. When doing so,
and if you need to grant that environment access to your Github account (for example, to clone a private repository), 
be sure to use a [deploy key](https://developer.github.com/v3/guides/managing-deploy-keys/) instead of a traditional 
SSH key. 

## NPM and published libraries
When creating a module to NPM enable 2FA for the publishing and settings update following the recommedations stated above.
