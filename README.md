# tuftex
### Dennis Evangelista, 2023
tuftex is a Latex package (not class) implementing tufte-latex stuff for compatibility with tufte.css, <https://edwardtufte.github.io/tufte-css/> and <https://github.com/edwardtufte/tufte-css>.

It is based on tufte-latex, <https://github.com/Tufte-LaTeX/tufte-latex> and <https://ctan.org/pkg/tufte-latex?lang=en>. Those are great, especially classes `tufte-handout` and `tufte-book` but they do not work right with `tex4ebook`, which I would like to use in order to create reflowable EPUB and iBooks that can be used on iPads for teaching etc. The things in tufte-latex that don't seem to play nice are soul and letterspace. Also, it's really hard to read the older Latex code so I'm trying to refactor it based on 2023 latex2e conventions. I'm doing it as a package vice a class because it's more of a style rather than a difference class of thing than an article or whatever.

## Desired workflows
The refactored tuftex shoudl be compatible with the following:
* Call pdflatex or latexmk for regular PDF production. I'm not super interested in odd flavors of Latex and I'm too lazy to implement many of the options I don't plan to use (sfcaptions, a4paper, etc etc etc). I would like the PDFs to print nicely double sided for hardcopy bound output.
* Call tex4ebook with an appropriate .cfg file and insert the tufte.css file to get nice reflowable iPad iBook output for when I don't want to print and carry around paper.

## Dependencies
Top level dependencies in Latex so far: 
* titlesec, titletoc
* sidenotes
* geometry
* ragged2e
* changepage
* mathpazo, helvet, beramono, fontenc, textcomp
* caption
* natbib
* bibentry
* pgffor

## Contributors
D Evangelista. 

## Thanks to
E Tufte, D Liepmann and team. 

