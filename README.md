![yo ast](https://user-images.githubusercontent.com/95488234/177071238-980b8b6d-0f5d-46fb-be6a-199daa3bfaa2.png)
<button>
<a href="https://www.linkedin.com/in/mauro-cocciolo" target="_blank"/>![ink](https://user-images.githubusercontent.com/95488234/177068790-c1c0ab81-9c62-4e98-9b9f-53e2637e8735.png)
profile</a>
</button>

### Hi there 👋


<!--
**Mauro-Cocciolo/Mauro-Cocciolo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
title: "Titulo de la presentacion"
subtitle: "Subtitulo de la presentacion"
author: "Autor de la presentacion"
fontsize: 9pt
date: \today
output:
  beamer_presentation:
    includes:
      in_header: mystyle1.tex
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo=FALSE, eval=TRUE)
```

## What is Rmarkdown

\centerline{\includegraphics[height=2.3in]{videoRmarkdown.png}}

To see the video please visit this url \alert{https://vimeo.com/178485416}

## Is RMarkdown useful?

\centerline{\includegraphics[height=2.3in]{RMarkdownOutputFormats.png}}

Yes, of course!

## Cheatsheet in Spanish

\centerline{\includegraphics[height=2.3in]{cheatsheet.png}}

\vspace{1cm}

You can find the cheatsheet in: \color{green} https://www.rstudio.com/wp-content/uploads/2015/03/rmarkdown-spanish.pdf

## Where can I learn about Rmarkdown?

\centerline{\includegraphics[height=2.5in]{study.png}}

Visit \alert{http://rmarkdown.rstudio.com/lesson-1.html}, there a lot of lesson to learn.

## Getting started
To work with R Markdown you need:

* Install [R](http://www.r-project.org/)
* Install the lastest version of [RStudio](http://rstudio.org/download/)
* Install the latest version of the `knitr` package: `install.packages("knitr")`
* Install latex if your output is in beamer format

# First section

## Creando secciones y slides
1. Las secciones se crean escribiendo `#` y luego el nombre de la seccion.

2. Los slides se crean escribiendo `##` y luego el titulo del slide.

## Incluyendo urls

- Se pueden incluir directamente escribiendo la url: http://rmarkdown.rstudio.com/

- Se pueden incluir asi: [YouTube](https://www.youtube.com/).

## Ordered list

1. Item 1
2. Item 2
3. Item 3
    + Item 3a
    + Item 3b
    
## Unordered list

* Item 1
* Item 2
    + Item 2a
    + Item 2b

## Showing R code
To include R code we can use chunk code.

```{r echo=TRUE, eval=FALSE}
x <- rnorm(n=100, mean=170, sd=15)
hist(x)
```

## Showing and evaluating R code
To include R code we can use chunk code.

```{r echo=TRUE, eval=TRUE, fig.width=4, fig.height=4}
x <- rnorm(n=100, mean=170, sd=15)
hist(x, col='salmon')
```

## Options for echo and eval inside a chunk code

- `echo`: if FALSE, knitr will not display the code in the code chunk above it’s results in the final document.

- `eval`: if FALSE, knitr will not run the code in the code chunk.

## Including external code
We can include external code writting it:

1. betweewn two `~~~~~~~`

2. between `\begin{verbatim}` and `\end{verbatim}`

Example using `~~~~~~~`.

~~~~~~~
if (a > 3) {
  u <- runif(n=a)
}
~~~~~~~

Example using `verbatim`.

\begin{verbatim}
if (a > 3) {
  u <- runif(n=a)
}
\end{verbatim}

# Second section

## Files
There are 3 types of files to produce this slides.

1. `plantilla1.Rmd`: where you write the slides.
2. `mystile1.tex`: where you configure your output beamer in a usual way.
3. Logo and figures in \alert{.png} format.

\vspace{1cm}

\centerline{\includegraphics[height=1.7in]{files.png}}

# Third section

## Justifying paragraphs

El siguiente parrafo __no__ esta justificado.

Los antófilos (Anthophila, gr. ‘que aman las flores’), conocidos comúnmente como abejas, son un clado de insectos himenópteros, sin ubicación en categoría taxonómica, dentro de la superfamilia Apoidea. Se trata de un linaje monofilético con más de 20 000 especies conocidas. Las abejas, al igual que las hormigas, evolucionaron a partir de avispas. Los antepasados de las abejas eran miembros de la familia Crabronidae y eran depredadores de insectos. Es posible que las primeras abejas se hayan alimentado del polen que cubría a algunas de sus presas y que, gradualmente, hayan empezado a alimentar a sus crías con polen en vez de insectos.

\justifying

Cuando se escribe un parrafo compuesto por varias lineas es usual que los finales de cada linea no coincidad. Para lograr que este parrafo se vea justificado fue necesario incluir al inicio el comando `\justifying`. \alert{Este parrafo si esta justificado}.

## Miscellaneous

- \emph{Sample Text}
- \textbf{Sample Text}
- \textit{Sample Text}
- \textsl{Sample Text}
- \alert{Sample Text}
- \textrm{Sample Text}
- \textsf{Sample Text}
- \color{green} Sample Text
- \structure{Sample Text}

## Slide with pauses
To include pauses we use `. . .`, 3 dots with spaces.

Example:

Content before the pause

. . .

Content after the pause
