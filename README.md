Class files for my research documents at the Utrecht University of Applied Science. Consists of a hu class file (a variant for shorter articles will be added at a later stage) and a wrapper around the biblatex package activating APA style (required) and fixing some common errors when using APA with Polyglossia. Also includes a beamer wrapper class called hu-presentatie now.

# hu.cls

## Requirements
* XeLaTeX
* Memoir class

## Options
All memoir options are passed through, with the following exceptions:
* `12pt` replaces `10pt` as default
* `nocolour` disables the coloured headings and links
* `dutch` will translate the title page / logo into dutch and sets the polyglossia language (defaults to English)
* `chaprecto` preserves Memoir's default behaviour of starting chapters on a recto page. Disabled by default.

## Commands
* `\subtitle{}` - a subtitle
* `\documenttype{}` - will show its content on the title page between guillemets; used for describing the various document types required for different projects
* `\version{}` - allows version information (or anything else) to be displayed at the bottom of the title page, above the logo
* `\author{}{}{}` - multiple authors can be added by multiple `\author{}` calls; accepts three arguments for given name, family name, and student number
* `\teacher{}{}` - multiple teachers can be added by multiple `\teacher{}` calls; accepts two arguments for given name and family name
* `\fac{}` - used to change the default Faculty of Nature and Technology / Faculteit Natuur en Techniek to something else

# hu-presentatie.cls

## Requirements
* XeLaTeX
* Beamer class

## Options
All beamer options are passed through, with the following exception:
* `dutch` will translate the logo into dutch and sets the polyglossia language (defaults to English)
