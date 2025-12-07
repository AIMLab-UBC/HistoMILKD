# HistoMILKD: A Multiple Instance Learning based Multi-Teacher Knowledge Distillation Framework for Whole Slide Image Classification

The IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) 2026

Mayur Mallya, Ali Khajegili Mirabadi, Hossein Farahani, Ali Bashashati

## Introduction

Foundation models (FM) in digital pathology have revolutionized the field of whole slide image (WSI) analysis, with models such as UNI, Virchow, Prov-GigaPath, and many more outperforming the previously established benchmarks set by the ImageNet-based backbones. 
However, despite several benchmarking studies, there has been no clear consensus on the choice of a single FM that is best suited for a variety of histopathology datasets and/or tasks. With more than 25 pathology FMs in the literature so far, the challenge of model selection is a growing concern.
Although an ensemble of FMs can circumvent this issue, given the bulky nature of individual FMs, the inference time and computational cost drastically increase with the addition of each FM into the ensemble. 

To this end, we propose $\textbf{HistoMILKD}$, the first multi-teacher knowledge distillation (MKD) framework for WSI classification. To handle the gigapixel resolution of WSIs, we use multiple instance learning (MIL), making this also the first work to integrate MIL and MKD frameworks into a single model. Our approach leverages the complementary representations of different FMs to distill collective task-specific knowledge into a single trainable MIL adapter on top of the student FM, which is utilized during inference.
Evaluated on five public datasets, the proposed approach significantly ($p<0.05$) outperforms the individual FMs, their ensemble, and previous MKD approaches in WSI classification.

Codes related to this research will be published in this repository.
