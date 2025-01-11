---
title: Pubblicare su un sito Github
created: 2025-01-11
author:
  - Paolo Volterra
tags:
  - io
  - appunti
  - Github
  - sito
  - quarto
  - Git
---
# Come Pubblicare su un sito Github

si lavora con 2 tipi di files:
- yaml
- qmd

**devono essere configurati** :
- git
- github



## Quarto

```

- quarto create-project paolovolterra.github.io --type website
- quarto preview
- quarto render

```

- INPUT: i qmd devono stare nella cartella post
- OUTPUT: gli output renderizzati da Quarto finiranno nella cartella docs

## Github


### pagina https://github.com/paolovolterra/paolovolterra.github.io/settings/pages 
- configurare il **main branch"

- creare un token per l'accesso automatico [HowTo](https://docs.github.com/en/organizations/managing-programmatic-access-to-your-organization/setting-a-personal-access-token-policy-for-your-organization#restricting-access-by-personal-access-tokens) 

![[Pasted image 20250111112443.png]]

### Git
- git remote remove origin
- git add docs
- git remote add origin https://github.com/paolovolterra/paolovolterra.github.io
- git remote -v

```bash
origin  https://github.com/paolovolterra/paolovolterra.github.io (fetch)
origin  https://github.com/paolovolterra/paolovolterra.github.io (push)
```

## Riferimenti

- [Il mio primo blog post](https://aborruso.github.io/til/un-sito-in-quarto/)con Quarto [[Il mio primo blog post – aborruso’s website]]
- [Creating your personal website using Quarto](https://ucsb-meds.github.io/creating-quarto-websites/)  con Quarto [[Creating your personal website using Quarto]]
- [Creating a Website (dal sito ufficiale)](https://quarto.org/docs/websites/)
- [Creating a Blog (dal sito ufficiale)](https://quarto.org/docs/websites/website-blog.html)
- [MEDS Computing Requirements & Software Installation Guide](https://ucsb-meds.github.io/MEDS-installation-guide/) con RStudio


![[Pasted image 20250111120036.png|200]]  ![[Pasted image 20250111120332.png|200]]
## Bibtex
https://www.getbibtex.com/


@misc{aborrusoPrimoBlog,
	author = {Andrea Borruso},
	title = {{I}l mio primo blog post – aborruso’s website --- aborruso.github.io},
	howpublished = {\url{https://aborruso.github.io/til/un-sito-in-quarto/}},
	year = {},
	note = {[Accessed 11-01-2025]},
}

@misc{marvinschmittCreateYour,
	author = {Marvin Schmitt},
	title = {{C}reate {Y}our {W}ebsite with {Q}uarto: {C}omplete {T}utorial and {T}emplate --- marvinschmitt.com},
	howpublished = {\url{https://marvinschmitt.com/blog/website-tutorial-quarto/}},
	year = {},
	note = {[Accessed 11-01-2025]},
}

@misc{adtariePersonalWebsite,
	author = {A.A. Wijaya},
	title = {{P}ersonal {W}ebsite using {J}upyter {N}otebook and {Q}uarto – {F}oreland of {T}houghts --- adtarie.net},
	howpublished = {\url{https://adtarie.net/posts/007-quarto-python-tutorial/}},
	year = {},
	note = {[Accessed 11-01-2025]},
}
