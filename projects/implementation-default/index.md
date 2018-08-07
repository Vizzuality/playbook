# **Implementation Defaults**


# Motivation:

As part of our objectives around improving performance and client value in the next three months we will create user stories and acceptance tests associated with tasks and functionalities. [There’s a separate guide outlining our approach to that here.](https://vizzuality.github.io/playbook/projects/stories-and-acceptance-tests/)

There’s a concern around the need to be comprehensive in such stories and tests, and about how to go about populating them (what things should be taken for granted unless stated otherwise, even if they are not specified in the user story/acceptance test)

The following list is not comprehensive and is subject to growth as we progress. The items are in no particular order:


## User Login
_Design, frontend, backend_

Whenever it is required for users to be able to log into a site they should also have the means to logout, cancel their registration and change their password.

If the user email is used for log in there should always be a confirmation sent to the user to verify they own the email and that it’s correct.

## Authentication required for pages
_Design, frontend, backend_
Whenever an unauthenticated user clicks to enter a page that requires authentication, the application should redirect to a login page (not overlay) and redirect back to the previous page after login.

## Storing user email
_Design, frontend, backend_
Whenever there’s a need to store user emails there should be a confirmation sent to the email. User’s should also have the means to change the email (in case they misspell it) and re-send the confirmation email. No other emails (subscriptions, newsletters, communications) should be sent to the user until they have confirmed their address

## Browser compatibility
_Design, frontend_
By default, and unless stated otherwise, all our projects should support the two latest versions of major desktop browsers (Chrome, Firefox, Safari, Explorer/edge) and iOS/Android in mobile

## Device compatibility
_Design, frontend_
By default, and unless stated otherwise, all projects should be browsable in desktops, tablets and mobile phones. Specific functionalities may vary across them. Please ask if in doubt

## Error pages
_Design, frontend, backend_
All server error pages (404, 500, 502, etc) should be styled according to the site’s visual guidelines, and provide understandable information, plus a link to the site’s home and the previous page.

## Runtime errors
_Frontend_
Whenever there’s a runtime error in the application there should be a visual cue that tells the user that something went wrong.  Visual elements such as spinners, loaders or page overlays should stop to allow the user to navigate out of the page or retry.

## Image size optimization
_Frontend_
All images should be optimized for internet usage in size

## Crawler protection for unpublished sites
_Frontend_
All staging and unpublished sites should have a valid [robots.txt](http://www.robotstxt.org/robotstxt.html) to avoid crawlers indexing them until publication

## SEO defaults
_Frontend, backend_
All public sections of sites should contain the minimum set of SEO friendly tags [TBD]
