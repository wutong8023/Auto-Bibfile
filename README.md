# Auto-Bibfile
Auto-Bibfile is an automatic toolkit for README.md generation based on bibtex file.

This repository is maintained by [Tongtong Wu](https://wutong8023.site). Please don't hesitate to collaborate or fix some entries. The automation script of this repo is partially adapted from [Automatic_Awesome_Bibliography](https://github.com/TLESORT/Automatic_Awesome_Bibliography).

## Quick Start
install:
```pip install bibtexparser```

run:
```python scripts/bibtex_to_md.py```

Click [here](https://github.com/wutong8023/Auto-Bibfile/tree/master/your_topic4all) for an exemplar.

## Instruction
1. check [bibtex.bib](https://github.com/wutong8023/Auto-Bibfile/blob/master/bibtex.bib): Auto-Bibfile will parse the keywords and meta-info of each entry.
2. the keywords should be predefined in [scripts/bibtext_to_md.py # fined_taxonomy](https://github.com/wutong8023/Auto-Bibfile/tree/master/scripts/bibtex_to_md.py#L84-L137).
3. check ```TODOs``` in [scripts/bibtext_to_md.py](https://github.com/wutong8023/Auto-Bibfile/blob/master/scripts/bibtex_to_md.py#L23) for customization.

## How to Contribute
Please feel free to use and share [Auto-Bibfile](https://github.com/wutong8023/Auto-Bibfile.git). It would be great 
if you mention it in your own repository by adding:
> The automation script of this repo is <br> powered by \[Auto-Bibfile\](https://github.com/wutong8023/Auto-Bibfile.git).
