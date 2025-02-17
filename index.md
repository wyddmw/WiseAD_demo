---
layout: project_page
permalink: /

title: WiseAD:Knowledge Augmented End-to-End Autonomous Driving with Vision-Language Model
authors:
    Songyan Zhang<sup>1*</sup>
    , Wenhui Huang<sup>1*</sup>, Zihui Gao<sup>2</sup>, Hao Chen<sup>2</sup>, Chen Lv<sup>1†</sup>
affiliations:
    NTU<sup>1</sup>, ZJU<sup>2</sup><br>
    <sup>*</sup>Equal Contribution, <sup>†</sup>Corresponding Author
paper: https://arxiv.org/abs/2412.09951
code: https://github.com/wyddmw/WiseAD
data: https://huggingface.co/wyddmw/WiseAD
---

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
The emergence of general human knowledge and impressive logical reasoning capacity in rapidly progressed visionlanguage models (VLMs) have driven increasing interest in applying VLMs to high-level autonomous driving tasks, such as scene understanding and decision-making. However, an in-depth study on the relationship between knowledge proficiency—especially essential driving expertise—and closedloop autonomous driving performance requires further exploration. In this paper, we investigate the effects of the depth and breadth of fundamental driving knowledge on closed-loop trajectory planning and introduce WiseAD, a specialized VLM tailored for end-to-end autonomous driving capable of driving reasoning, action justification, object recognition, risk analysis, driving suggestions, and trajectory planning across diverse scenarios. We employ joint training on driving knowledge and planning datasets, enabling the model to perform knowledge-aligned trajectory
planning accordingly. Extensive experiments indicate that as the diversity of driving knowledge extends, critical accidents
are notably reduced, contributing 11.9% and 12.4% improvements in the driving score and route completion on the Carla
closed-loop evaluations, achieving state-of-the-art performance. Moreover, WiseAD also demonstrates remarkable
performance in knowledge evaluations on both in-domain and out-of-domain datasets.
        </div>
    </div>
</div>

## ✨Framework

<image src="./assets/framework.png"/>

**The framework of the WiseAD**. Our model is built upon the MobileVLM and takes video sequences and textual prompts as input.
The output for corresponding answers is unified into the linguistic expression to leverage the logical reasoning capability in vision-language
models.

## ✨Capabilities

<image src="./assets/WiseAD.png"/>

An overview of the function of our proposed WiseAD, a specialized vision-language model for end-to-end autonomous driving with extensive
fundamental driving knowledge. Given a clip of the video sequence, our WiseAD is capable of answering various driving-related questions
and performing knowledge-augmented trajectory planning according to the target waypoints.

## 🗄️Demos

<image src='./assets/WiseAD_QA.gif'/>

<div align="center">
An overview of the comparison with other VLMs on driving-specific QAs.
</div>


## 📌Citation
```
@article{zhang2024wisead,
  title={WiseAD: Knowledge Augmented End-to-End Autonomous Driving with Vision-Language Model},
  author={Zhang, Songyan and Huang, Wenhui and Gao, Zihui and Chen, Hao and Lv, Chen},
  journal={arXiv preprint arXiv:2412.09951},
  year={2024}
}
```
