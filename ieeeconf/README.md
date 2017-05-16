# ieeeconf Template

Template using the ieeeconf conference document class.

# Template Variables

Variables have two potential configuration points, which will be described here. The first point is the frontmatter variable name, which is used by the underlying system to identify the value at build time. The second point is the placeholder value, which can be replaced during the new command, or manually edited later. For the following description, variables will be named in the format `Variable Name, Placeholder Name - Description`

## MultiMarkdown Frontmatter

1. `latex author`,`$AUTHOR` - name of the paper author
2. `latex title`, `$TITLE` - title of the document
3. `bibtex`, `$BIBTEX` - defines the Bibtex file to process for this document. Delete this line to eliminate bibliography support
5. `my abstract` - `$ABSTRACT` - location of the abstract file
6. `my acknowledgments` - `$ACKNOWLEDGMENTS` - if included, the location of the acknowledgments file
6. `my packages` - `$PACKAGES` - if included, injects the contents of this file into the document before the document begins, allowing additional packages or LaTeX options to be defined.

## LaTeX Variables

These variables are not included in the frontmatter by default, since they aren't always in use. Some of these variables require being defined in a LaTeX file (e.g. the packages file) due to requiring LaTeX commands.

1. `my columns` - defines the number of columns for the document to use, defaulting to `onecolumn` if undefined.
2. `my doc class` - defines the document style to use, either `conference` (default) or `journal`.
3. `my size` - defines the size of text to use. For example, IEEE Transactions paper use `9pt`, while most papers use `10pt` (default).
4. `my association` - if included, association of the paper author(s). This will require being defined in a LaTeX file.
5. `my keywords` - keywords for this document
6. `my appendix` - if included, appendix(ces) for the document. This will require being defined in a LaTeX file.
7. `my biography` - if included, biography(ies) for the document. This will require being defined in a LaTeX file.
8. `my top margin`, `my bottom margin` - if set, sets the margin for the given side of the page. If only one is set, the value is used for both.
9. `my inner margin`, `my outer margin` - if set, sets the margin for the left/right side of the page. If only one is set, the value is used for both.
