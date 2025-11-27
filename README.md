# Old article LaTeX code

**This is almost entirely taken from this [excellent
repository](https://github.com/proafxin/antique_book)**. I just made a few
style changes to make it more in line with articles of the time. All the
heavy lifting, such as the excellent font design, is done by the linked
repository. 

### List of changes made (off the top of my head):

- Changed page margins to `[margin=1in]`
- Removed line underneath header with `\renewcommand{\headrulewidth}{0pt}`
- Fixed a double period after subsections
- Redefined section/subsection design in line with those from the time in
  economic journals such as *The Quarterly Journal of Economics* and *The
  Economic Journal*
- Odd/even page number split
- Removed neon coloring around hyperlinks in `.pdf` output by setting  
`[hidelinks]` argument in `hyperref` package.
- Added user-configurable SHORT TITLE that can be defined in the main
  `.tex` file. Previously this was defined as the section header. 
- May have made a few other changes. Exact changes can be seen by comparing
  `antiquebook.cls`. 
    - If you wish to make any further adjustments, this is the file to
      edit.

### A few important notes

- From the original repo: Try to place the files in the
  project directory rather than putting them in the texlive/miktex
  installation directory to make it globally accessible. Otherwise you may
  break your system.

- **THIS PACKAGE WILL NOT WORK UNLESS YOU COMPILE WITH XELATEX**
    - The `.pdf` output will still work. It just will be in plain boring
      Computer Modern font and you'll be wondering what the point was of
      installing this.
    - In order to get the nice old fonts etc., you must change your LaTeX
      compilation engine from the default `pdflatex` to `xelatex`. 
      For VimTeX users, I have added the magic comment 
      `%! TeX engine = xelatex` so it should work on first run. 

Huge thank you to the original author of this package. It is really
incredible how similar the typeface looks to articles from the 1930s. 
