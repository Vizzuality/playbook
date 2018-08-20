# Import files preparation

These are our recommendations for preparation of data files for import into a database and which we use when reviewing them.

1. CSV format;
2. UTF8-encoded;
3. Data organised in rows rather than columns or rows + columns:
    - Computers process files row by row, making this the easiest structure from perspective of writing importer code;
    - This is most easily achieved when data is modelled into entity (object) types and each file only represents a single entity type;
    - Entity types are often the nouns you would use when describing the data, e.g. "a list of **policies** with attached **instruments**, each with its specific **indicators**" (the bold items are the entities);
    - Data which is partly pivoted (e.g. by year or by indicator) violates the above rule and is generally not recommended for structuring import files, because it increases the complexity of parsing files. If such organisation is useful to be applied, that must be done consistently throughout the dataset.
4. First row is reserved for column names;
5. Files should not contain "noise" such as:
    - empty rows;
    - empty columns;
    - annotations.
6. Column names should be short and consistent in style:
    - Where a column represents an attribute of an entity, e.g. indicator name or unit, those names should be simple, short and consistent in style across files (e.g. all lower case and using underscores like "unit", "display_name", etc);
    - Where a column is used to pivot data, e.g. by year or indicator (which is generally not recommended as described above), the column name should still be short and consistent in style across files, meaning that if we need to e.g. create a column for a value of an indicator with a long name, the column name should **not** be the full name of the indicator but a short name (sometimes called "code" or "slug"), which is mapped to the full name in a separate dictionary / metadata file.
7. A single cell should generally contain a single value (a number, one string of text etc);
    - If it contains more than one, it might mean two entity types are represented in a single spreadsheet, which typically is an indication that data needs to be split between two sheets with "child" referencing "parent" by some kind of unique key;
    - Sometimes it is acceptable to have more than one value in a cell, for example in cases where we want to express a relationship between one entity of type A and more than one entity of type B and we do not need any other attributes to describe that association. In such case the convention is to use a semicolon-separated list of keys.
8. Missing data is best represented by absence of data, i.e. empty cell;
9. Where data contains numeric indicator values:
    - It is often a good idea to include a metadata file with indicator name + unit and a short name ("code" or "slug"), which is referenced in other sheets;
    - It is important for the unit to be part of the data / metadata, rather than be embedded in the file name or column name.
10. Where the data contains formatted text:
    - It is best to format it in markdown. This also applies where text does not need rich formatting, but needs to be displayed in paragraphs;
    - It is good to be aware that some characters might exist in multiple variations in heterogeneous source files. For example, there are ~15 unicode characters that are different flavours of quotation marks. For purposes of consistent presentation, those are best unified;
    - Spelling and capitalisation variations are often a cause of duplicate records in the database. Where a text is repeated across rows in the import file it helps to pay attention to keeping it consistent (e.g. "and" vs "&", typos, inconsistent punctuation etc);
    - Repetition of this kind may also be an indication of a need to split the spreadsheet, creating a "dictionary".
11. Where data references locations:
    - Location names should not appear directly in data files, instead codes should be used to reference them;
    - To reference countries it is best to use standardised three letter iso codes;
    - Regions, country groupings and sub-national units require a dictionary file which establishes unique codes for those entities, so that data files can reference the codes instead of full names (e.g. `geoid | name | type`)
12. Files should contain only data that is meant to be imported, rather than all available data;
13. The fewer files, and the more consistent in structure, the better. Often a few spreadsheets with related / similarly structured data can be combined into a single one by adding a column to meaningfully differentiate between the rows.
