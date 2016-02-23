# syllabus

## Credits:

This syllabus was adapted from [Benjamin Schmidt](https://github.com/bmschmidt/syllabus) who adapted his code from [Andrew Goldstone](https://github.com/agoldst/tex).
Instead of forking I started new repo since I did too many changes.

## The "interface"

`make syllabus.pdf` makes the PDF using pandoc, xelatex, and biber.

`make syllabus.html` makes HTML. (It does not work for me)

`make clean` cleans up the truly astonishing number of intermediate files this process generates.

## Getting just the syllabus template and not the rest of agoldst/tex

If you want subdirectories as a repo, then you need the following command to strip away all of a repo except for a subdirectory. Please seach for "Making a Subdirectory the New Root" in [Pro Git, chapter 6, section 4](http://www.ctan.org/tex-archive/help/Catalogue/entries/biblatex.html). Example below is for getting tex folder from [Andrew Goldstone](https://github.com/agoldst/tex)'s repo.

```
git clone agoldst/tex
cd tex
git filter-branch --subdirectory-filter syllabus HEAD 
```

