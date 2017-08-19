markdown-cv-oo
===========

This repository reflects the changes I made over [elipapa's](https://elipapa.github.io/) [markdown-cv](http://elipapa.github.io/markdown-cv) project. Please visit the original repository for instructions regarding web use.

### What's different?

I assume you have seen the output of @elipapa's template. I think he did a very good job in separating the CV content and style, enabling users to edit a plain text file to obtain a pretty decent looking CV. I built on his repository to modify the template for my personal use and for a little bit of a CSS practice.

I moved away from the monospace font choice towards what @kjhealy suggested in his LaTeX template. I also introduced a couple CSS tags in index.md. Currently, these added CSS tags require this document to be rendered with kramdown.

This is how it looks right now:

![Web view of the CV](https://github.com/oguzhanogreden/markdown-cv/blob/oopatch/outputs/screen.png)

### What is to be improved?

- ~~Mail and webpage links are not vertically centered between the surrounding elements.~~
- ~~The positioning of dates for education, awards and publications are "absolute" (in CSS terms). This prevents a nice output when different screen resolutions are used. Moreover, one can only use dates which are formatted as YYYY-YYYY.~~ _(I viewed my CV in LaTeX while considering this point. I concluded that dates are not as important to have their own column and can be pushed beneath the titles.)_
- ~~Finally, I'm leaving the code temporarily with some discrepancy between web view and PDF view.~~
  - I want to inroduce a difference as to how the contact information is presented in digital form and print form.
- I'm not perfectly happy with the asymmetric gaps resulting from e.g. the lack of descenders in "Trinity" and presence of ascenders in "Fellow".

### Original Author

Eliseo Papa ([Twitter](http://twitter.com/elipapa)/[GitHub](http://github.com/elipapa)/[website](https://elipapa.github.io)).

### Licenses

[MIT License](https://github.com/oguzhanogreden/markdown-cv/blob/master/LICENSE) and [OFL licences](https://github.com/oguzhanogreden/markdown-cv/blob/oopatch/fonts/Crimson_Text/OFL.txt) for all of the included fonts.
