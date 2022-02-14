# Auto-Bibfile
Auto-Bibfile is an automatic toolkit for README.md generation based on bibtex file.

## Quick Start
- Install: 
```pip install bibtexparser```
  
- Update the configuration in [scripts/config.py](https://github.com/wutong8023/Auto-Bibfile/blob/master/scripts/config.py).

- Add a new paper: 
paste a bib entry to [bibtex.bib](https://github.com/wutong8023/Auto-Bibfile/blob/master/bibtex.bib).

- Run: 
```python scripts/run.py```  (click [HERE](https://github.com/wutong8023/Auto-Bibfile/tree/master/your_topic4all) to see a demo.
)

- Categorize:
Add ```keywords``` to each entry and write down your note within ```@String()```. For example,

```latex
@inproceedings{wu2022pretrained,
  title={Pretrained Language Model in Continual Learning: A Comparative Study},
  author={Tongtong Wu and Massimo Caccia and Zhuang Li and Yuan-Fang Li and Guilin Qi and Gholamreza Haffari},
  booktitle={Proceedings of ICLR},
  year={2022},
  url={https://openreview.net/forum?id=figzpGMrdD},
  keywords={
        Empirical Study,
        NLP,
        Supervised Learning,
        Sequence Classification,
        Catastrophic Forgetting,
        PLMs,
        MAVEN, CLINC150, WEBRED,
  },
}
@String(wu2022pretrained="To explore the layer-wise property of pretrained languge models in continual learning, we thoroughly compare the continual learning performance over the combination of 5 PLMs and 4 veins of CL methods on 3 benchmarks in 2 typical incremental settings.")
```

## Instruction
1. Update [bibtex.bib](https://github.com/wutong8023/Auto-Bibfile/blob/master/bibtex.bib): Auto-Bibfile will parse the keywords and meta-info of each entry.
2. The keywords **MUST** be predefined in [scripts/config.py # fined_taxonomy](https://github.com/wutong8023/Auto-Bibfile/tree/master/scripts/config.py#L20-L73), but feel free to update what you need.
3. Update [scripts/config.py](https://github.com/wutong8023/Auto-Bibfile/blob/master/scripts/config.py) for customization.

## How to Contribute
Please feel free to use and share [Auto-Bibfile](https://github.com/wutong8023/Auto-Bibfile.git). It would be great 
if you can mention it in your repository by adding:
> The automation script of this repo is powered by \[Auto-Bibfile\](https://github.com/wutong8023/Auto-Bibfile.git).

## Acknowledgement
This repository is developed and maintained by [Tongtong Wu](https://wutong8023.site). The automation script of this repo is partially adapted from [Automatic_Awesome_Bibliography](https://github.com/TLESORT/Automatic_Awesome_Bibliography).
