
LaTeX paper format for the NeurIPS 2019
=======================================

This is an example of a paper in LaTeX for the conference NeurIPS 2019, but it could be also useful for future editions of a such conference.

Be careful, revision process is double blinded, so, at submittion you shoud omit the author names.

I didn't use natbib because it produces some conflicts with other packages.


## Modifications of the original format ##

I modified the next in order to have a better visualization but using the format and instructions given by NerurIPS committee.

### Modification 1. ### 

Replace :

```
\usepackage[final]{neurips_2019}
```

with:

```
\usepackage[nonatbib, final]{neurips_2019}

```

### Modification 2. ###

Add the package:

```
\usepackage{cite}
```

### Modification 3. ###

In order to add multiple authors in a better visualization, I used:

```
\author{
  \textbf{AuthorName AuthorSurname $^1$, AuthorName AuthorSurname $^1$} \\ 
  \textbf{AuthorName AuthorSurname $^1$ $^2$, AuthorName AuthorSurname $^2$}
  \\
  $^1$ Deppartament1, University1, Country1 \\ 
  $^2$ Deppartament2, University2, Country2 \\
  \texttt{\{email1, email2, email3\}@affiliation.edu} 
  \\
  \texttt{email4@affiliation.edu} 
}
```

### Modification 4. ###

Cite the papers using ```\cite{reference-name}```, example:

```
... we used the Caffe framework \cite{reference1}.
```

### Modification 5. ###

I added the next packages in order to have a better manage of the images.

```
\usepackage{float}
\usepackage{graphicx}
\usepackage{subfig}
```

### Modification 6. ###

Replace all the References section (included the subtitle) with:

```
\bibliography{references}{}
\bibliographystyle{plain}
```

## Compiling ##

Compile step by step as follows:

Step 1. Compite with PDFLaTeX

Step 2. Compile with BibTeX

Step 3. Compile with PDFLaTeX

Step 4. Compile with PDFLaTeX


## Optional: Submiting to ArXiV ##

Be careful when you submit your paper to ArXiV.

Submit the main LaTeX files in a .tag compressed file. In my case, such main files are: paper_neurips.tex, neurips_2019.sty, images (folder), paper_neurips.bbl (generated from the references.bib at Step 2 of compiling).


## About ##

By: Dennis Núñez-Fernández

Website: [http://dennishnf.com](http://dennishnf.com)

