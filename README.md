# Bibtex source for Deoplete

| :warning: WARNING :warning:                                                                              |
|:--------------------------------------------------------------------------------------------------------:|
| This is just a placeholder. The repository is located here: https://gitlab.com/spadarian/deoplete_bibtex |

Deoplete-bibtex is a source for [Deoplete](https://github.com/Shougo/deoplete.nvim) which helps you manage your references for a document.

![Demo](https://gitlab.com/spadarian/deoplete_bibtex/-/raw/master/img/demo.png)

The main motivation to make this source is depicted in the figure above. In that example, the keyword is `padarian` (my last name) and the completion list not only contains the IDs that contain my last name but also all the publications where I'm a co-author. The source effectively matches the title, authors and year of publication.

At the moment, the source is not configurable but I will change that in the near future. Of course, any PR are welcome.

This source is heavily based on [deoplete-biblatex](https://github.com/lionawurscht/deoplete-biblatex).

## Installation

1. Install [deoplete](https://github.com/Shougo/deoplete.nvim#install).
2. Install [bibtexparser](https://bibtexparser.readthedocs.io/en/master/install.html#how-to-install).
3. Install this source using your favourite method.

## Examples

In `tex` files:

```
\bibliography{path,../ref/path} 
```

In `markdown` files:

```
---
...
bibliography:
  - path
  - ../ref/path
...
---
```

## Features

* Search for bib files within the current document (in the bibliography section).
* Re-load references from files that have changed since last check.
* Matches references by title, authors and year of publication.
* Preview window with extra information about the selected reference.

![Demo](https://gitlab.com/spadarian/deoplete_bibtex/-/raw/master/img/info.png)
