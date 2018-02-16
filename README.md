kjh-vita-markdown
===========

I tried to mimic the famous [kjh-vita](https://github.com/kjhealy/kjh-vita) LaTeX template in Markdown, using CSS. You can see the live example [here!](https://oguzhanogreden.github.io/markdown-cv/)

![demo](/media/demo.png)

This repo is simply some changes over [@elipapa](https://github.com/elipapa)'s [markdown-cv](http://elipapa.github.io/markdown-cv) repo. I would definitely check his version too.

## How to use?

[@elipapa](https://github.com/elipapa/) wrote [very clear instructions](https://elipapa.github.io/markdown-cv/) for publishing your CV using this template. Please first check them.

Using the template is pretty easy if you like it as it is :-) Take a side-by-side look at the [example](/index.html) page and the [`index.md`](/index.md). What you _need_ to modify is staring at you!

In case there are things you do not like, your markdown and CSS skills are the limit. I listed some of the easily modifiable things in case you want a quick route.

1. Do you want to print and/or be friendly to people who may print your CV?  
  - **If yes,** adjust the `PRINT ADDRESS BOX` section. Make sure CSS tags such as `{:id='web-email'}` are next to the corresponding lines.  
  - **If no,** remove the section or comment it out.
2. Do you want to have email, linkedin, github links under your title?
  - **If yes,** adjust the `WEB ADDRESS BOX` section. If you want more, search for `web-email` in [`cv-print.css`](/media/cv-print.css) and repeat the pattern.
  - **If no,** remove the section or comment it out.
3. Do you want to have columns in your skills section?  
  - **If yes,**  do you want to get rid of the title-like looking first lines?
    - **If yes,** Then search for `SKILLS TITLE STYLE` in [`cv-screen.css`](/media/cv-screen.css) and remove/comment the relevant code block. 
  - **If no,** you can just remove everything and type your skills. Do not forget to add the `{: et}` tag _(I trust that you checked [`index.md`](/index.md) :-))_.
4. Do you want to add lines below the phone and mail of your references?
  - **If yes,** search for `REFERENCES ICONS` in [`cv-screen.css`](/media/cv-screen.css) and increment the integers in `nth-last-of-type(1)` and `nth-last-of-type(2)`.

## Why?

I used to keep my CV in LaTeX, using kjh-vita template. The source included entries like this:

~~~ latex
\marginhead{\sffamily {education}}

\ind M.Sc., Methodology \& Statistics for Behavioral, Biomedical and Social Sciences, \\ Utrecht University, The Netherlands, September 2015 - June 2017.\\ \hspace{0.35in} 

Thesis: \emph{Variable Selection Strategies in Multinomial Prediction Models}. \\
\normalsize \vspace{0.05in}
~~~

Now the same entry looks like this:

~~~ markdown
M.Sc. __Methodology & Statistics__, Utrecht University
{: et}
`2015 - 2017`
- Thesis title: 'Variable selection strategies in multinomial prediction models'
~~~

---

Seeing [@elipapa](https://github.com/elipapa)'s template, I wanted to use it with a different style. The result is satisfying to me. Markdown code became more complex but I think it is a fair price to pay for what I got. It was good CSS practice as well :-)

### What is to be improved?

1. I'm not perfectly happy with the asymmetric gaps resulting from e.g. the lack of descenders in "Trinity" and presence of ascenders in "Fellow".

### Licenses

Significant portion of the code was published by Eliseo Papa ([website](https://elipapa.github.io)) under
[MIT License](https://github.com/oguzhanogreden/markdown-cv/blob/master/LICENSE).

All the included fonts are licensed under [OFL](https://github.com/oguzhanogreden/markdown-cv/blob/oopatch/fonts/Crimson_Text/OFL.txt).
