# Report Template

Template using the report document class.

# Template Variables

Variables have two potential configuration points, which will be described here. The first point is the frontmatter variable name, which is used by the underlying system to identify the value at build time. The second point is the placeholder value, which can be replaced during the new command, or manually edited later. For the following description, variables will be named in the format `Variable Name, Placeholder Name - Description`

## MultiMarkdown Frontmatter
1. `latex author`,`$AUTHOR` - name of the paper author
2. `latex title`, `$TITLE` - title of the document
3. `bibtex`, `$BIBTEX` - defines the Bibtex file to process for this document. Delete this line to eliminate bibliography support

## LaTeX Variables

These variables are generally not exposed by MMD frontmatter, since the variables use special LaTeX commands which are sanitized by MMD. In order to control these, it is generally easiest to create a LaTeX file (conventionally, `metadata.tex`) and include the file by inserting the following line into the frontmatter:
```
latex input: metadata.tex
```

1. `latex author`, `$AUTHOR` - name of the paper author
2. `latex title`, `$TITLE` - title of the document
3. `my abstract` - if this LaTeX variable is defined, include the contents of the file named as the abstract.
4. `my packages` - if defined, includes the contents of the specified file into the document preamble, allowing custom packages to be introduced.
