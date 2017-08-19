markdown-cv-oo
===========

This repository reflects the changes I made over [elipapa's](https://elipapa.github.io/) [markdown-cv](http://elipapa.github.io/markdown-cv) project. Please visit the original repository for instructions regarding web use.

### What's different?

I assume you have seen the output of @elipapa's template. I think he did a very good job in separating the CV content and style, enabling users to edit a plain text file to obtain a pretty decent looking CV. I built on his repository to modify the template for my personal use and for a little bit of a CSS practice.

I moved away from the monospace font choice towards what @kjhealy suggested in his LaTeX template. I also introduced a couple CSS tags in index.md. Currently, these added CSS tags require this document to be rendered with kramdown.

This is how it looks right now:

![Web view of the CV](https://github.com/oguzhanogreden/markdown-cv/blob/oopatch/outputs/screen.png)

### What is to be improved?

- Mail and webpage links are not vertically centered between the surrounding elements.
- The positioning of dates for education, awards and publications are "absolute" (in CSS terms). This prevents a nice output when different screen resolutions are used. Moreover, one can only use dates which are formatted as YYYY-YYYY. 
- Finally, I'm leaving the code temporarily with some discrepancy between web view and PDF view.

The most interesting part for me is of course the second item, as it will require me to improve my command of CSS.

### Original Author

Eliseo Papa ([Twitter](http://twitter.com/elipapa)/[GitHub](http://github.com/elipapa)/[website](https://elipapa.github.io)).

![Eliseo Papa](https://s.gravatar.com/avatar/eae1f0c01afda2bed9ce9cb88f6873f6?s=100)

### Licenses

[MIT License](https://github.com/oguzhanogreden/markdown-cv/blob/master/LICENSE) and [OFL licences](https://github.com/oguzhanogreden/markdown-cv/blob/oopatch/fonts/Crimson_Text/OFL.txt) for all of the included fonts.
