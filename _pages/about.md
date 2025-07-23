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
I am currently pursuing a Master's degree at the <a href="http://www.vsislab.com"><font color="#4169E1">Visual Sensing and Intelligent Systems Laboratory (VSISLab)</font></a>, Shandong University, China, with a focus on Computer Vision and Deep Learning. I am advised by <a href="https://ieeexplore.ieee.org/author/37085379581"><font color="#4169E1">Prof. Wei Zhang</font></a>, and I also work closely with my co-supervisors <a href="https://faculty.sdu.edu.cn/songran/en/index.htm"><font color="#4169E1">Prof. Ran Song</font></a> and <a href="https://scholar.google.com/citations?user=fjmxqlUAAAAJ&hl=zh-CN"><font color="#4169E1">Prof. Xiao Jia</font></a>. Before this, I received my Bachelor's degree in Automation from Shandong University.
</p>

<p style="text-align: justify;">
<span style="color: #a7b529;"><strong>Research Interests:</strong></span> I am broadly interested in the field of computer vision and deep learning. Particularly, I have mostly focused on <strong>visual scene understanding from images and videos</strong>. I have worked in <strong>image understanding tasks</strong> (Object Detection, Semantic Segmentation, Object Tracking), <strong>video understanding tasks</strong> (Exo-Centric Videos, Ego-Centric Videos, Human Activity Detection), and <strong>vision-language modeling</strong>. I am also very interested in <strong>medical image analysis</strong> and have worked on <strong>medical image segmentation tasks</strong> and <strong>medical surgical scene understanding tasks</strong>, among others. 
</p>

<p style="text-align: justify;">
<span style="color: #c59428;"><strong>Collaboration:</strong></span> I am always open to discussions and collaborations. Please feel free to reach out via email if you're interested. 
</p>

# 🔥 News
- *2025.06*: &nbsp;🎉🎉 Our team won 2nd place at the **ATPOS 2025 Big Data Competition**.
- *2024.11*: &nbsp;🎉🎉 Our team won the National Second Prize in the **Huawei Cup** China Graduate Mathematical Modeling Contest.
- *2023.06*: &nbsp;🎉🎉 Our team won 1st place at the **SoccerNet Action Spotting** Challenge at the CVSports workshop during CVPR 2023.

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/B2Q-Net.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[B2Q-Net: Bidirectional Branch Query Network for Online Surgical Phase Recognition](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)

**Wenjie Zhang**, Zhiheng Li, Yue Bi, Xiao Jia, Ran Song, Yipeng Zhang, and Wei Zhang

<strong><font color="#4169E1">Preprints</font></strong>

This work introduced a novel method, named B2Q-Net, which formulates the online phase recognition task as the bidirectional query between phase-level features and frame-level features. Extensive evaluations on three datasets demonstrate that B2Q-Net consistently outperforms state-of-the-art methods in recognition accuracy while achieving an inference speed of 106 fps.

<details>
<summary>Abstract</summary>

Surgical phase recognition (SPR) is essential for surgical workflow analysis and provides immediate guidance during procedures. In contrast to offline recognition, which processes videos post-operatively, online phase recognition (OPR) requires real-time inference without relying on future frames. Existing methods aggregate frame-level information into a global representation and treat the task as frame-wise classification. However, this pipeline lacks a feedback mechanism for integrating historical information into local temporal modeling. To address this limitation, we propose the Bidirectional Branch Query Network (B2Q-Net), which reformulates the OPR task as the bidirectional query between phase-level features and frame-level features. B2Q-Net incorporates historical information during the initialization of phase queries. This enables bidirectional information flow during iterative refinement of two-level feature maps between phases and frames. Furthermore, we introduce a dual-scale selector (DSS) to generate high-quality phase queries for the current video clip. These phase queries retrieve historical information from the proposed state space query (SSQ) module, which uses learnable tokens as the historical state space to preserve historical information. Extensive evaluations on three datasets demonstrate that B2Q-Net consistently outperforms state-of-the-art methods in recognition accuracy while achieving an inference speed of 106 fps.

</details>

</div>
</div>

- [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020**

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
- *2025.05* Shandong University May Fourth Youth Science Award.
- *2023.06* Shandong Province Outstanding Graduate (Undergraduate).
- *2022.01* First Prize in the Shandong Province Undergraduate Science and Technology Innovation Competition.
- *2021.11* First Class Academic Scholarship, Shandong University.

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
