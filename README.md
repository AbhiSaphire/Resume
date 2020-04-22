## Resume
My LaTex based Resume.


## Credit
[**LaTeX**](http://www.latex-project.org) is a fantastic typesetting program that a lot of people use these days, especially the math and computer science people in academia.

[**LaTeX FontAwesome**](https://github.com/furl/latex-fontawesome) is bindings for FontAwesome icons to be used in XeLaTeX.

[**Roboto**](https://github.com/google/roboto) is the default font on Android and ChromeOS, and the recommended font for Google’s visual language, Material Design.

[**Source Sans Pro**](https://github.com/adobe-fonts/source-sans-pro) is a set of OpenType fonts that have been designed to work well in user interface (UI) environments.


## Prerequisite
You should need an updated version of texlive (to include Source Sans Pro Font).

It is however not in the official repository for 12.04 and 12.10, so you have to add an unofficial one: 
```
$ sudo add-apt-repository ppa:texlive-backports/ppa
```
After that, you can install TexLive with apt, not forgetting to get the font package:
```
$ sudo apt-get install texlive
$ sudo apt-get install texlive-fonts-recommended texlive-fonts-extra
```
You can now use Source Sans Pro:
```cls
\newcommand*{\footerfont}{\sourcesanspro}
\newcommand*{\bodyfont}{\sourcesanspro}
\newcommand*{\bodyfontlight}{\sourcesansprolight}
```

## How to Run
You are now ready to convert your tex into pdf file by :
```
xelatex resume.tex
```
