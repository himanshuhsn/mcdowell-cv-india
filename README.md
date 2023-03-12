# McDowell CV
McDowell CV is a LuaLaTeX class for building neat and space-efficient CVs using the design originally proposed by Gayle L. McDowell at 
http://www.careercup.com/resume. 

The class is based on `article` class. The paper format is set to U.S. letterpaper by default. A template showing an example usage of the class is included.

## Screenshot
<img src="https://github.com/himanshuhsn/mcdowell-cv-india/blob/master/McDowell_CV.png" width="240px"/>

## Use with Overleaf
<img src="https://ucbe9456bbfce83bc61a5f4cb014.dl.dropboxusercontent.com/cd/0/inline/B4EmTqMV32JrmcKkSGzzE5sQRWwPHphgmkPYDE2a6uogU8vP4N_8JB3rX5cqgcZQtP7t9Ex_WHCkDLVQJdyg8FRSrpbnmibvHTBewo0VKdEBGjM0UtXmkv4Jdt4q2cwQflKPHRBVDsDN7mnJWI234JrBpPXtvbeWTeyB4KhPQ2Jg-Q/file#"/>

Above image not displaying? 🥲 Check the image [here](https://www.dropbox.com/s/q4j3yj8iforn4z2/mcdowell-cv-overleaf-use.gif?raw=1).

## Use Cases
- A great tool making it easy to build CVs: https://latexresu.me/.

## Class Options
 - `calibri` - sets calibri as the main font. Otherwise the default font is Times New Roman since version 1.1.0.

## Commands
The class features the following commands:
 - `\name{name}` - defines the applicant's name to be printed by `\printheader`.
 - `\address{address}` - defines the applicant's address to be printed by `\printheader`.
 - `\contacts{contacts}` - defines the applicant's contacts to be printed by `\printheader`.
 - `\makecvheader` - prints the CV header consisting of the name (see the `\name` command), address (see the `\address` command) and contacts (see the `\contacts` command).
 
## Environments
 - `\begin{cvsection}{sectionname}` - prints a section with a header consisting of the name in bold small caps and a page-wide horizontal line below.
 - `\begin{cvsubsection}[linesnum]{left}{center}{right}{content}` - prints a subsection with header consisting of the `left`, `center` and `right` titles. The optional `linesnum` argument defines the amount of lines in the header. The argument only affects the vertical spacing between the environment header and content thus eliminating the effect of *tabu* package vertical spacing bug.

## Build Instructions
- Make sure `lualatex` (see http://www.luatex.org/download.html) is installed on your machine and is available in the terminal or a command line client of your choice.
- In the terminal or a command line client of your choice, go to the folder containing `McDowell_CV_Template.tex` and `mcdowellcv.cls`, and run the following command: `lualatex McDowell_CV_Template.tex`.
