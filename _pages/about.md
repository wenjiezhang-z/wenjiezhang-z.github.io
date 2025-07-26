---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# 👤 About Me
<p style="text-align: justify;">
Hello! I am currently pursuing a Master's degree at the <a href="http://www.vsislab.com"><font color="#4169E1">Visual Sensing and Intelligent Systems Laboratory (VSISLab)</font></a>, Shandong University, China, with a focus on Computer Vision and Deep Learning. I am advised by <a href="https://ieeexplore.ieee.org/author/37085379581"><font color="#4169E1">Prof. Wei Zhang</font></a>, and I also work closely with my co-supervisors <a href="https://faculty.sdu.edu.cn/songran/en/index.htm"><font color="#4169E1">Prof. Ran Song</font></a> and <a href="https://scholar.google.com/citations?user=fjmxqlUAAAAJ&hl=zh-CN"><font color="#4169E1">Prof. Xiao Jia</font></a>. Before this, I received my Bachelor's degree in Automation from Shandong University.
</p>

<p style="text-align: justify;">
<span style="color: #a7b529; font-size: 1.1em; font-weight: bold;">Research Interests:</span> I am broadly interested in the field of computer vision and deep learning. Particularly, I have mostly focused on <strong>visual scene understanding from images and videos</strong>. I have worked in <strong>image understanding tasks</strong> (Object Detection, Semantic Segmentation, Object Tracking), <strong>video understanding tasks</strong> (Exo-Centric Videos, Ego-Centric Videos, Human Activity Detection), and <strong>vision-language modeling</strong>. I am also very interested in <strong>medical image analysis</strong> and have worked on <strong>medical image segmentation tasks</strong> and <strong>medical surgical scene understanding tasks</strong>, among others. 
</p>

<p style="text-align: justify;">
<span style="color: #c59428; font-size: 1.1em; font-weight: bold;">Collaboration:</span> I am always open to discussions and collaborations. Please feel free to contact me if you're interested. 
</p>

<p style="text-align: justify; margin-top: 20px; margin-bottom: 20px;">
🎓 <span style="color: #000000; font-size: 1.1em; font-weight: bold;">I am currently looking for a PhD position starting in Fall 2026. If you are interested, please feel free to contact me.</span></p>

# 🔥 News
- *2025.06*: &nbsp;🎉🎉 Our team won 2nd place at the **ATPOS 2025 Big Data Competition**.
- *2024.11*: &nbsp;🎉🎉 Our team won the National Second Prize in the **Huawei Cup** China Graduate Mathematical Modeling Contest.
- *2023.06*: &nbsp;🎉🎉 Our team won 1st place at the **SoccerNet Action Spotting** Challenge at the CVSports workshop during CVPR 2023.

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/B2Q-Net.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**B2Q-Net: Bidirectional Branch Query Network for Online Surgical Phase Recognition**](https://arxiv.org/)

<span style="font-size: 1.1em; font-weight: bold;">Wenjie Zhang</span>, Zhiheng Li, Yue Bi, Xiao Jia, Ran Song, Yipeng Zhang, and Wei Zhang

<strong><font color="#4169E1">Preprints</font></strong>

This work introduced a novel method, named B2Q-Net, which formulates the online phase recognition task as the bidirectional query between phase-level features and frame-level features. Extensive evaluations on three datasets demonstrate that B2Q-Net consistently outperforms state-of-the-art methods in recognition accuracy while achieving an inference speed of 106 fps.

<div style="display: flex; align-items: center; margin-bottom: 1em;">
<details class="abstract-details" style="margin-right: 10pt;">
<summary class="abstract-summary-button">[<span class="custom-underline">Abstract</span>]</summary>
<br>
<p style="text-align: justify;">
Surgical phase recognition (SPR) is essential for surgical workflow analysis and provides immediate guidance during procedures. In contrast to offline recognition, which processes videos post-operatively, online phase recognition (OPR) requires real-time inference without relying on future frames. Existing methods aggregate frame-level information into a global representation and treat the task as frame-wise classification. However, this pipeline lacks a feedback mechanism for integrating historical information into local temporal modeling. To address this limitation, we propose the Bidirectional Branch Query Network (B2Q-Net), which reformulates the OPR task as the bidirectional query between phase-level features and frame-level features. B2Q-Net incorporates historical information during the initialization of phase queries. This enables bidirectional information flow during iterative refinement of two-level feature maps between phases and frames. Furthermore, we introduce a dual-scale selector (DSS) to generate high-quality phase queries for the current video clip. These phase queries retrieve historical information from the proposed state space query (SSQ) module, which uses learnable tokens as the historical state space to preserve historical information. Extensive evaluations on three datasets demonstrate that B2Q-Net consistently outperforms state-of-the-art methods in recognition accuracy while achieving an inference speed of 106 fps.
</p></details>
<a href="https://github.com/vsislab/B2Q-Net" class="code-link">[Code]</a>
</div>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/DBR-TAD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**DBR-TAD: Diffusion-Based Boundary Refinement for Temporal Action Detection**](https://arxiv.org/)

<span style="font-size: 1.1em; font-weight: bold;">Wenjie Zhang</span>, Zhiheng Li, Wenhao Tan, Ran Song, Jiyu Cheng, and Wei Zhang

<strong><font color="#4169E1">Preprints</font></strong>

This work introduced a diffusion-based boundary refinement method for TAD. DBR-TAD locates accurate action boundaries from noisy action boundaries through a progressive denoising process. Extensive experiments demonstrate that DBR-TAD achieves the state-of-the-art performance on three single-label datasets and two multi-label datasets.

<div style="display: flex; align-items: center; margin-bottom: 1em;">
<details class="abstract-details" style="margin-right: 10pt;">
<summary class="abstract-summary-button">[<span class="custom-underline">Abstract</span>]</summary>
<br>
<p style="text-align: justify;">
Existing temporal action detection (TAD) methods take videos of different lengths as input and produce a fixed-length feature sequence by feature extraction and temporal downsampling, followed by action boundary localization and action classification. However, the temporal downsampling often leads to the loss of action information and results in the difficulty of locating accurate action boundaries. To address this issue, we introduce DBR-TAD, a diffusion-based boundary refinement method for TAD. DBR-TAD locates accurate action boundaries from noisy action boundaries through a progressive denoising process. Its core component is the diffusion-based boundary refinement (DBR) module, which progressively converts the distributions corresponding to uncertain and noisy action boundaries predicted by any TAD model to the specific distributions corresponding to good action boundaries. Extensive experiments demonstrate that DBR-TAD achieves the state-of-the-art performance on three single-label datasets and two multi-label datasets.
</p></details>
<a href="https://github.com/wenjiezhang-z/DBR-TAD" class="code-link">[Code]</a>
</div>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/FAM.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**FAM: Frequency-Based Adaptive Mutual Learning for Semi-Supervised Medical Image Segmentation**](https://arxiv.org/)

Yue Bi, <span style="font-size: 1.1em; font-weight: bold;">Wenjie Zhang</span>, Xiao Jia, Zhongwei Zhao, Ran Song, Nengwang Yun, and Wei Zhang

<strong><font color="#4169E1">Preprints</font></strong>

This work introduced a novel framework designed to enhance the reliability and self-correction capability of pseudo-labels. FAM tackles confirmation bias by incorporating multiple strategies, with distinct inner and outer learning loops designed for progressive optimization. Extensive experiments on the ACDC and PROMISE12 datasets demonstrate that FAM achieves state-of-the-art performance.

<div style="display: flex; align-items: center; margin-bottom: 1em;">
<details class="abstract-details" style="margin-right: 10pt;">
<summary class="abstract-summary-button">[<span class="custom-underline">Abstract</span>]</summary>
<br>
<p style="text-align: justify;">
Co-training has proven to be a powerful framework for semi-supervised medical image segmentation, primarily leveraging pseudo-labeling via cross-supervision. A persistent challenge in existing co-training methods is confirmation bias, where inaccurate pseudo-labels are reinforced, leading to unstable training. To address this issue, we propose Frequency-based Adaptive Mutual Learning (FAM), a novel framework designed to enhance the reliability and self-correction capability of pseudo-labels. FAM tackles confirmation bias by incorporating multiple strategies, with distinct inner and outer learning loops designed for progressive optimization. In the inner learning loop, Mutual Uncertainty Distance (MUD) is introduced to reduce the uncertainty gap between labeled and unlabeled data, improving pseudo-label reliability and mitigating error accumulation. In the outer learning loop, we introduce Adaptive Self-Correction (ASC), an adaptive strategy that refines subnet updates based on pseudo-label quality, enabling self-correction and improving training stability. The entire training process is supported by the Frequency Dual-View Stream (FDvS) architecture, which leverages the frequency tendencies of both networks and images, providing complementary feature representations that enhance both inner and outer learning. Extensive experiments on the ACDC and PROMISE12 datasets demonstrate that FAM achieves state-of-the-art performance, highlighting its effectiveness in semi-supervised medical image segmentation. 
</p></details>
<a href="https://github.com/biyue1207/FAM.git" class="code-link">[Code]</a>
</div>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/TriQuery.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**TriQuery: A Query-Based Model for Surgical Triplet Recognition**](https://arxiv.org/)

Mengrui Yao, <span style="font-size: 1.1em; font-weight: bold;">Wenjie Zhang</span>, Lin Wang, Fufang Wang, Zhong Zhao, and Xiao Jia

<strong><font color="#4169E1">Preprints</font></strong>

This work introduced TriQuery, a query-centric model for surgical triplet recognition and classification. Built on a multi-task Transformer framework, TriQuery decomposes the complex triplet task into three semantically aligned subtasks using task-specific query tokens, which are processed through specialized attention mechanisms. 

<div style="display: flex; align-items: center; margin-bottom: 1em;">
<details class="abstract-details" style="margin-right: 10pt;">
<summary class="abstract-summary-button">[<span class="custom-underline">Abstract</span>]</summary>
<br>
<p style="text-align: justify;">
Artificial intelligence has shown great promise in advancing intelligent surgical systems. Among its applications, surgical video action recognition plays a critical role in enabling accurate intraoperative understanding and decision support. However, the task remains challenging due to the temporal continuity of surgical scenes and the long-tailed, semantically entangled distribution of action triplets composed of instruments, verbs, and targets. To address these issues, we propose TriQuery, a query-centric model for surgical triplet recognition and classification. Built on a multi-task Transformer framework, TriQuery decomposes the complex triplet task into three semantically aligned subtasks using task-specific query tokens, which are processed through specialized attention mechanisms. We introduce a Multi-Query Decoding Head (MQ-DH) to jointly model structured subtasks and a Top-K Guided Query Update (TKQ) module to incorporate inter-frame temporal cues. Experiments on the CholecT45 dataset demonstrate that TriQuery achieves improved overall performance over existing baselines across multiple classification tasks. Attention visualizations further show that task queries consistently attend to semantically relevant spatial regions, enhancing model interpretability. These results highlight the effectiveness of TriQuery for advancing surgical video understanding in clinical environments.
</p></details>
</div>

</div>
</div>

<span class='anchor' id='-academic-projects'></span>
# ⚙️ Academic Projects

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Academic_Projects/kindergarten.gif' alt="Smart Campus Personnel Safety System Demo" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<strong><font color="#4169E1">Smart Campus Personnel Safety Behavior Analysis and Early Warning System</font></strong>

<p style="text-align: justify;">
This project addresses the pressing need for digital and intelligent management upgrades in campus administration. Key functionalities include intruder detection for campus fences, a student dangerous behavior alert system, and a classroom behavior management system that monitors.
</p>

- *The algorithm has been deployed at Qingya Kindergarten in Huaiyin District, Jinan, China.*
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Academic_Projects/bird.gif' alt="Intelligent Bird Repellent System Demo" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<strong><font color="#4169E1">Intelligent Bird Repellent System</font></strong>

<p style="text-align: justify;">
This project tackles an issue in power infrastructure: the detrimental impact of birds perching and nesting on power grid towers, which results in both bird electrocution and costly power grid trips. To proactively mitigate these hazards, we've developed a laser bird repellent system based on <strong>YOLOv5 + DeepSORT</strong>.
</p>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Academic_Projects/Rebar.jpg' alt="Rebar Tensile Strength Qualification Detection Demo" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<strong><font color="#4169E1">An Image Recognition-Based System for Rebar Tensile Strength Qualification Detection</font></strong>

<p style="text-align: justify;">
This system leverages advanced image processing and deep learning techniques to automatically assess the quality of steel rebar after tensile testing. By providing precise and consistent qualification detection, the system can help reduce human error, accelerate material verification, and ultimately contribute to safer and more reliable infrastructure.
</p>

</div>
</div>


# 🏅 Honors and Awards
- [*2025.06*]&nbsp;&nbsp;&nbsp;&nbsp;2nd place at the ATPOS 2025 Big Data Competition.
- [*2025.05*]&nbsp;&nbsp;&nbsp;&nbsp;May Fourth Youth Science Award of Shandong University.
- [*2024.11*]&nbsp;&nbsp;&nbsp;&nbsp;2nd Prize in the Huawei Cup National Graduate Mathematical Modeling Contest.
- [*2023.06*]&nbsp;&nbsp;&nbsp;&nbsp;1st place at the SoccerNet Action Spotting Challenge at the CVSports workshop during CVPR 2023.
- [*2023.06*]&nbsp;&nbsp;&nbsp;&nbsp;Shandong Province Outstanding Undergraduate Graduate.
- [*2022.01*]&nbsp;&nbsp;&nbsp;&nbsp;1st Prize in the Shandong Province Undergraduate Science and Technology Innovation Competition.
- [*2021.11*]&nbsp;&nbsp;&nbsp;&nbsp;1st Class Academic Scholarship, Shandong University.

# 📖 Educations

<div style="display: flex; align-items: flex-start; gap: 20px; border: 1px solid #eee; padding: 15px; border-radius: 8px; background-color: #fff;">
    <div style="flex-shrink: 0; width: 150px;">
        <img src='images/Shandong_University.jpg' alt="Shandong University Logo" style="max-width: 100%; height: auto; display: block; border-radius: 4px;">
    </div>
    
    <div>
        <p style="margin: 0 0 5px 0; font-weight: bold; font-size: 1.1em;">Shandong University</p>
        <p style="margin: 0 0 5px 0;"><strong>Position:</strong> Master of Science (M.Sc.) in Control Science and Engineering</p>
        <p style="margin: 0 0 5px 0;"><strong>Under:</strong> Prof. Wei Zhang</p>
        <p style="margin: 0 0 5px 0;"><strong>Thesis:</strong> Query-based Surgical Scene Understanding</p>
        <p style="margin: 0;"><strong>Period:</strong> Sep 2023 - Present</p>
    </div>
</div>

<div style="display: flex; align-items: flex-start; gap: 20px; border: 1px solid #eee; padding: 15px; border-radius: 8px; background-color: #fff;">
    <div style="flex-shrink: 0; width: 150px;">
        <img src='images/Shandong_University.jpg' alt="Shandong University Logo" style="max-width: 100%; height: auto; display: block; border-radius: 4px;">
        </div>
    
    <div>
        <p style="margin: 0 0 5px 0; font-weight: bold; font-size: 1.1em;">Shandong University</p>
        <p style="margin: 0 0 5px 0;"><strong>Position:</strong> Bachelor of Technology (B.Tech) in Automation</p>
        <p style="margin: 0 0 5px 0;"><strong>Under:</strong> Prof. Wei Zhang</p>
        <p style="margin: 0 0 5px 0;"><strong>Thesis:</strong> Human Action Recognition with Attention Mechanism</p>
        <p style="margin: 0;"><strong>Period:</strong> Sep 2019 - Jun 2023</p>
        </div>
</div>

<br>
<br>

<div style="text-align: center;">
    <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=hB9vJPVf8Tiu-4VYekyixCzGDZbWUwu5E8TdfQqEI90&cl=ffffff&w=300"></script>
</div>

<br>
