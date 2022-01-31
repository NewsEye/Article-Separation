# Article Separation

## Description
Article separation (AS), also called article segmentation, is the process of dividing a newspaper page into its articles. So far, existing systems still need considerable input from human users to solve this task due to handcrafted rules that need parameter tuning to work well dependent on the layout of the newspaper page. In the context of the NewsEye project the aim is to create an automated workflow that is independant from any user input. 

## Workflow
The preceeding tasks 2.1 Layout Analysis (LA) and 2.2 Automated Text Recognition (ATR) in the NewsEye project provide geometrical information in the form of text lines / baselines and the corresponding transcription of the text. This information we want to use to solve the AS task by combining traditional LA methods, semantic information and machine learning based approaches.

Tasks 2.1 and 2.2 are processed and further developed in the [Transkribus](https://transkribus.eu/) platform which has its roots in the FP7 Project [tranScriptorium](http://transcriptorium.eu/) (2013-2015) and was further developed in the H2020 Project [READ](https://read.transkribus.eu/) (2016-2019). 

The Transkribus GitHub repository can be found at https://github.com/transkribus/.

## Used models and algorithms
* Seq2Seq models for ATR: [Paper](https://arxiv.org/abs/1903.07377)
* ARU-Net / Pixel labeling: [GitHub Repository](https://github.com/TobiasGruening/ARU-Net) - [Paper](https://arxiv.org/abs/1802.03345)
* Stroke Width Transform: [Paper](https://ieeexplore.ieee.org/document/5540041)
* DBScan: [GitHub Repository](https://github.com/chrisjmccormick/dbscan) - [Paper](https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf)
* BERT: [Paper](https://arxiv.org/abs/1810.04805)
* Graph Neural Networks: [Paper](https://persagen.com/files/misc/scarselli2009graph.pdf)

## Data
To our knowledge, there is no general AS dataset on newspaper pages on which a comparison with other existing workflows is possible.

## CITlab AS GitHub Repository:
The code for the article separation can be found in the following GitHub repository, which was updated for M45:
https://github.com/CITlabRostock/citlab-article-separation-new
