

## Table Category
* [Collection of VQA papers](#papers)
* [Leaderboard](#vqa-challenge-leaderboard)
* [Tutorials](#Tutorials)
* [VQA Dataset](#Dataset)
* [VQA Algorithm](#Algorithm)
* [VQA Code Library](#CodeLibrary)

## :page_facing_up:Collection of Papers
  - VQA: https://github.com/jokieleung/awesome-visual-question-answering/blob/master/README.md#CVPR-2020
  - Text-VQA https://github.com/xinke-wang/Awesome-Text-VQA

  - Survey papers:
    - KB-VQA: https://github.com/astro-zihao/Awesome-KBQA
    - 2019, V+L dataset and methods: https://arxiv.org/pdf/1907.09358.pdf
    - 2017, VQA dataset and methods: https://www.sciencedirect.com/science/article/pii/S1077314217300772?casa_token=EX_Gt8Ib5rQAAAAA:NSFjlS4iVem0eC_iQCvHf6HPkg18fbQAQC-BqxW96u85bg2gMNw0yFFUFS4HvdiAuzr0D0FQ1Bc

## :green_book: Tutorials
  - Sigir2020: https://www.avishekanand.com/talk/sigir20-tute/
  - CVPR2020 (Recent Advances in Vision-and-Language Research): https://rohit497.github.io/Recent-Advances-in-Vision-and-Language-Research/
  - KDD 2020 (Scene Graph) https://suitclub.ischool.utexas.edu/IWKG_KDD2020/slides/Shih-Fu.pdf

## :chart_with_upwards_trend: Leaderboard
  - VQAv2 leaderboard: https://visualqa.org/roe.html
  
|  Algorithm | Accuracy  |
|  ----  | ----  |
| Renaissance	|79.34|
|UNIMO Ensemble||
|  VinVL (MSR+MS Cog Svcs., X10 models ) ([paper](https://arxiv.org/pdf/2101.00529.pdf),[code](https://github.com/pzzhang/VinVL)) | 76.60 |  
|  GridFeat+MoVie | 76.36  |
| [DL-61 (BGN)](https://arxiv.org/pdf/1907.09815.pdf)  | 76.08 |
| VILLA (adversarial training) based on UNITER, ([paper](https://arxiv.org/pdf/2006.06195.pdf), [code](https://github.com/zhegan27/VILLA))|75.9|
| Ensemble LXMERT, VILBERT, VisualBERT |75.15|
| Pixel-BERT x152 |74.45|
|	Oscar([paper](https://arxiv.org/abs/2004.06165), [code](https://github.com/microsoft/Oscar))	|73.82|
|UNITER (+grid feature)([paper](https://arxiv.org/pdf/1909.11740.pdf), [code1](https://github.com/ChenRocks/UNITER),[code2](https://github.com/YIKUAN8/Transformers-VQA))	|73.82|
|SOHO|73.47|
|	LXMERT ([paper](https://arxiv.org/pdf/1908.07490.pdf),[code](https://github.com/airsplay/lxmert))	|72.54|
|	VLBERT	|72.22|
|	Pixel-BERT r50 |71.35|
|ViLT|71.32|
|	MCAN		|70.93|
|	VisualBERT 	|71.00|
|	ViLBERT	|70.92|
|	BUTD		|65.67|
|	MUTAN		|60.17|

- VizWiz leaderboard: https://evalai.cloudcv.org/web/challenges/challenge-page/523/leaderboard/1459#leaderboardrank-1

|  Algorithm | Accuracy  |
|  ----  | ----  |
|  [Alibaba](https://ivc.ischool.utexas.edu/~yz9244/VizWiz_workshop_2021/videos/Enhancing_Textual_Cues_VQA_5-minute.mp4) | 61.81  |
|  [HSSLab](https://ivc.ischool.utexas.edu/~yz9244/VizWiz_workshop_2021/videos/VIZWIZ_VQA_HSSLAB_INSPUR_Presentation.mp4)| 60.1  |
|  LXMBERT | 55.4  |
|  Pythia | 54.72  |
|  Gridfeature+MCAN | 54.17  |
|  VilBERT | 52  |
|  SAN  | 47.3  |

- Text VQA leaderboard (2021):https://eval.ai/web/challenges/challenge-page/874/leaderboard/2313

|  Algorithm | Accuracy  |
|  ----  | ----  |
|  Mia | 73.67  |
|  SunLan | 65.86  |
|  Summer | 59.16 |
|  [RUArt-M4C](https://arxiv.org/pdf/2010.12917v1.pdf) | 48.1 |
|  ST-VQA|45.66 |
|  M4C | 39.01  |
|  LoRRA | 27.63  |


## :floppy_disk: Dataset
* VQA Dataset
     * General VQA
          - COCO
          - VQAv1, VQAv2
          - VQA Dialog

     * Text-VQA
          - TextVQA
          - Scene Text VQA
          - OCR-VQA (toy-sized dataset, containing book/poster cover)
     * Doc-VQA
     * Re-ask VQA 
          - Inverse Visual QA (iVQA)
          - VQA-Rehrasings
          - VQA-LOL
          - VQA- introspect
     * Re-image VQA
          - VQAv2
          - VQA-CP
     * VQA reasoning
          - VCR (11/2018)
          - Visual Entailment(2019)
          - GQA
          - CLEVER
          - Referring Expression
          - NLVR2 (2018)
     * VQA with External Knowledge
          - OK-VQA
          - FVQA
          - KBVQA
          - KVQA (2019)
     * Explainable/Grounding Image Captioning/VQA
        - Grounding for image captioning (referring expression)
          - Flickr30K entities
          - Visual Genome
          - RefClef
          - RefCOCO 
          - CLEVER-Ref+
          - Google Referring expression
          - PhraseCut
        - grounding for VQA
          - Visual7W (2016) 
          - Visual Genome (2016) | [paper](http://visualgenome.org/static/paper/Visual_Genome.pdf) | [website](http://visualgenome.org/)
          - VQA-HAT(2016)
          - VQS (2017) | [paper](https://arxiv.org/pdf/1708.04686.pdf)
          - VQA-X(2018)
          - VQA-E(2018) 
## :pencil2: Algorithm
   * Image Feature preparation
      - Show, Attend and Tell  (2015/5)
      - SAN (2015/11)
      - BUTD (2017/7) | [paper](https://arxiv.org/pdf/1707.07998.pdf)
      - Grid Feature (2020/1)
      - Pixel-BERT (2020/4)
      - SOHO(2021/4)
      - VinVL(2021/4)
   * Enhanced multimodal fusion
      - Bilinear pooling: how to fuse two vectors into one
        - MCB (2016/6)
        - MLB (2016/10)
        - MUTAN (2017/5)
        - MFB&MFH (2017/8)
        - BLOCK (2019/1)
      - FiLM: Feature-wise Linear Modulation		
        - FiLM
      - cross-modal attention
        - SAN (2015/11)
        - HierCoAttn (2016/5)
        - DAN (2016/11)
        - DCN (2018/4)
        - BAN (2018/5)
      - pretraining:
        - UNITER
        - ViLBERT
        - LXMERT	
        - B2T2
        - VisualBERT
        - Unicoder-VL
        - VL-BERT
        - ERINE-ViL (AAAI, 2021): Scene Graph Prediction
        - Oscar
        - UNIMO (ACL, 2021)
      - End-to-End pretraining:
        - SOHO (CVPR, 2020/4)
        - ViLT (2021, ICML)
      - graph attention/graph Convolutional Network
        - Graph-Structured, (2016/9)
        - Relation Network, (2017/6)
        - Graph Learner,(2018/6)
        - MuRel, (2019/2)
        - ReGAT, (2019/3)
        - LCGN (2019/5)
      - Cross-modal+intra-modal
        - MCAN, 2019: Deep Modular Co-Attention Network

      - Multi-step reasoning
        - MAC: Memory, Attention and Composition

      - Neural module networks
        - NMN, (2015/11)
        - N2NMN,(2017/4)
        - PG+EE,(2017/5)
        - TbD,(2018/3)
        - stackNMN,(2018/7)
        - NS-VQA,(2018/10)
        - Prob-NMN, (2019/2)
        - MMN (2019/10)

   * External Knowledge Algorithm
      - Mucko (1/2020)
      - [KRISP (2020)](https://arxiv.org/pdf/2012.11014.pdf)
