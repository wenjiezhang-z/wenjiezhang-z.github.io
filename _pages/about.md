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
Hello! I am an Algorithm Engineer with the Foundation Model Team at <b>Li Auto</b>. I received my Master's degree in Control Science and Engineering from <b>Shandong University</b>, China, where I was a member of the <a href="http://www.vsislab.com">Visual Sensing and Intelligent Systems Laboratory (VSISLab)</a>, advised by <a href="https://ieeexplore.ieee.org/author/37085379581">Prof. Wei Zhang</a> and working closely with <a href="https://faculty.sdu.edu.cn/songran/en/index.htm">Prof. Ran Song</a> and <a href="https://scholar.google.com/citations?user=fjmxqlUAAAAJ&hl=zh-CN">Prof. Xiao Jia</a>. I also spent time as a research intern at the <b>OPPO Research Institute</b>, working on robots. Before that, I received my Bachelor's degree in Automation, also from Shandong University.
</p>

<div class="video-grid">
  <figure>
    <video controls muted playsinline preload="metadata">
      <source src="assets/oppo_nianhui_web.mp4" type="video/mp4">
      Your browser does not support the video tag. You can <a href="assets/oppo_nianhui_web.mp4">download the video</a> instead.
    </video>
    <figcaption>🎬 <b>Live show</b> — the robot performing on stage at the OPPO annual meeting.</figcaption>
  </figure>
  <figure>
    <video controls muted playsinline preload="metadata">
      <source src="assets/caipai_web.mp4" type="video/mp4">
      Your browser does not support the video tag. You can <a href="assets/caipai_web.mp4">download the video</a> instead.
    </video>
    <figcaption>🔧 <b>Rehearsal</b> — tuning the motions backstage before the show.</figcaption>
  </figure>
</div>

<p class="media-note">A robot I developed and debugged during my research internship at the OPPO Research Institute.</p>

<p style="text-align: justify;">
<span class="section-label" style="color: #a7b529;">Research Interests:</span> My work centers on <b>video and scene understanding</b> and on making it reliable enough for real-world deployment. So far this has spanned temporal action detection, online surgical workflow analysis, semi-supervised medical image segmentation, and, more recently, <b>embodied AI</b> for humanoid whole-body control. I am especially interested in <b>query-based architectures</b>, <b>generative refinement</b>, and models that stay accurate under real-time constraints.
</p>

<p style="text-align: justify;">
<span class="section-label" style="color: #c59428;">Collaboration:</span> I am always open to discussions and collaborations — feel free to reach out at <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a>.
</p>

<!--
<p style="text-align: justify; margin-top: 20px; margin-bottom: 20px;">
🎓 <span style="color: #000000; font-size: 1.1em; font-weight: bold;">I am currently looking for a PhD position starting from 2026 fall. If you are interested, please feel free to contact me. Here is my <a href="https://wenjiezhang-z.github.io/assets/files/CV_WenjieZhang_SDU.pdf">resume</a>.</span></p>
-->

# 🔥 News

- *2026.07*: &nbsp;🎉🎉 <span class="news-highlight">Started a new journey as an **Algorithm Engineer** with the **Foundation Model Team, Li Auto**.</span>
- *2026.05*: &nbsp;📄 **CodeAct** has been accepted by **IEEE Robotics and Automation Letters (IEEE RA-L)**.
- *2026.01*: &nbsp;📄 **B2Q-Net** has been accepted by **IEEE Transactions on Medical Imaging (IEEE TMI)**.
- *2025.10*: &nbsp;🥉 Won **3rd Place** (Bronze Medal) in the **Mecha Challenge (Robot Dance Championship)** at **IROS 2025**, Hangzhou.
- *2025.06*: &nbsp;🥈 Our team achieved **2nd Place** in the **APTOS 2025 Big Data Challenge**.
- *2024.11*: &nbsp;🏅 Awarded the **National 2nd Prize** in the **China Graduate Mathematical Modeling Contest (Huawei Cup)**.
- *2023.06*: &nbsp;🏆 Our team secured **1st Place** in the **SoccerNet Action Spotting Challenge** at the CVSports Workshop, **CVPR 2023**.

<span class='anchor' id='-publications'></span>
# 📝 Selected Publications

<!-- <p class="section-note">A selection of my work. For the complete and up-to-date list, please see my <a href="{{ site.author.googlescholar }}">Google Scholar profile</a>.</p> -->

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/CodeAct.png' alt="CodeAct framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**CodeAct: Codebook-Guided Multi-Skill Integration for Dynamic Humanoid Whole-Body Control**](https://ieeexplore.ieee.org/abstract/document/11539976)

Zhiheng Li, <span class="author-me">Wenjie Zhang</span>, Chengxin Liu, Mingxin Zhang, Xing Fang, Hang Zhong, Huaidong Zhou, and Ran Song

<span class="pub-venue">IEEE Robotics and Automation Letters (IEEE RA-L), IF: 5.3</span>

CodeAct is a two-stage imitation learning framework for humanoid robots that resolves training bias in multi-skill integration by leveraging structured expert codebooks and attention-guided priors, achieving strong performance both in simulation and in real-world deployment on a Unitree G1.

<div style="display: flex; align-items: center; margin-bottom: 1em;">
<details class="abstract-details" style="margin-right: 10pt;">
<summary class="abstract-summary-button">[<span class="custom-underline">Abstract</span>]</summary>
<br>
<p style="text-align: justify;">
Recent advances in humanoid robotics have showcased the potential of imitation learning (IL) to replicate dexterous whole-body behaviors in unstructured environments. However, conventional IL approaches that integrate multiple skills into a unified policy often suffer from training bias toward dominant or easily learned samples, resulting in a compromised action space that fails to preserve fine-grained dynamics of individual skills. To address this limitation, we propose CodeAct, a novel two-stage IL framework that facilitates multi-skill integration through structured expert code guidance. In the first stage, individual motions are distilled into high-fidelity expert codes, which are used to populate a dynamic codebook. In the second stage, a codebook-guided attention mechanism leverages these structured expert priors to constrain the optimization of the multi-skill policy. Importantly, expert codes serve as structured skill-specific representations, providing fine-grained supervision signals for different skills throughout multi-skill integration, thus helping reduce training bias and enabling seamless skill composition. Extensive experiments in simulation and on a real Unitree G1 humanoid robot demonstrate that CodeAct achieves competitive performance in both single-skill learning and multi-skill integration.
</p></details>
</div>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/B2Q-Net.png' alt="B2Q-Net architecture overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**B2Q-Net: Bidirectional Branch Query Network for Online Surgical Phase Recognition**](https://ieeexplore.ieee.org/document/11355439)

<span class="author-me">Wenjie Zhang</span>, Zhiheng Li, Yue Bi, Xiao Jia, Ran Song, Yipeng Zhang, and Wei Zhang

<span class="pub-venue">IEEE Transactions on Medical Imaging (IEEE TMI), IF: 12.4</span>

B2Q-Net reformulates online surgical phase recognition as a bidirectional query between phase-level and frame-level features. Evaluations on three datasets show that it consistently outperforms state-of-the-art methods in accuracy while running at 106 fps.

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


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/DBR-TAD.png' alt="DBR-TAD pipeline overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**DBR-TAD: Diffusion-Based Boundary Refinement for Temporal Action Detection**

<span class="author-me">Wenjie Zhang</span>, Zhiheng Li, Wenhao Tan, Ran Song, Jiyu Cheng, and Wei Zhang

<span class="pub-venue">Preprint</span>

DBR-TAD is a diffusion-based boundary refinement method for temporal action detection (TAD) that recovers accurate action boundaries from noisy ones through a progressive denoising process, achieving state-of-the-art performance on three single-label and two multi-label datasets.

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


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/FAM.png' alt="FAM framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**FAM: Frequency-Based Adaptive Mutual Learning for Semi-Supervised Medical Image Segmentation**

<span class="author-me">Wenjie Zhang</span>, Yue Bi, Xiao Jia, Zhongwei Zhao, Ran Song, Nengwang Yun, and Wei Zhang

<span class="pub-venue">Preprint</span>

FAM improves the reliability and self-correction capability of pseudo-labels in co-training. It mitigates confirmation bias through coupled inner and outer learning loops for progressive optimization, reaching state-of-the-art performance on the ACDC and PROMISE12 datasets.

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

<!-- 
<div class='paper-box'><div class='paper-box-image'><div><img src='images/Publication/TriQuery.png' alt="TriQuery framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**TriQuery: A Query-Based Model for Surgical Triplet Recognition**

Mengrui Yao, <span class="author-me">Wenjie Zhang</span>, Lin Wang, Fufang Wang, Zhong Zhao, and Xiao Jia

<span class="pub-venue">Preprint</span>

TriQuery is a query-centric model for surgical triplet recognition. Built on a multi-task Transformer, it decomposes the entangled triplet task into three semantically aligned subtasks via task-specific query tokens, each handled by a specialized attention mechanism.

<div style="display: flex; align-items: center; margin-bottom: 1em;">
<details class="abstract-details" style="margin-right: 10pt;">
<summary class="abstract-summary-button">[<span class="custom-underline">Abstract</span>]</summary>
<br>
<p style="text-align: justify;">
Artificial intelligence has shown great promise in advancing intelligent surgical systems. Among its applications, surgical video action recognition plays a critical role in enabling accurate intraoperative understanding and decision support. However, the task remains challenging due to the temporal continuity of surgical scenes and the long-tailed, semantically entangled distribution of action triplets composed of instruments, verbs, and targets. To address these issues, we propose TriQuery, a query-centric model for surgical triplet recognition and classification. Built on a multi-task Transformer framework, TriQuery decomposes the complex triplet task into three semantically aligned subtasks using task-specific query tokens, which are processed through specialized attention mechanisms. We introduce a Multi-Query Decoding Head (MQ-DH) to jointly model structured subtasks and a Top-K Guided Query Update (TKQ) module to incorporate inter-frame temporal cues. Experiments on the CholecT45 dataset demonstrate that TriQuery achieves improved overall performance over existing baselines across multiple classification tasks. Attention visualizations further show that task queries consistently attend to semantically relevant spatial regions, enhancing model interpretability. These results highlight the effectiveness of TriQuery for advancing surgical video understanding in clinical environments.
</p></details>
</div> -->

<!-- </div>
</div> -->

<!-- <span class='anchor' id='-experience'></span>
# 💼 Experience

<div class="edu-card">
  <div class="edu-card-body">
    <p class="edu-card-title">Li Auto</p>
    <p><strong>Role:</strong> Algorithm Engineer, Foundation Model Team</p>
    <p class="edu-card-meta">Jul 2026 – Present · Beijing, China</p>
  </div>
</div>

<div class="edu-card">
  <div class="edu-card-body">
    <p class="edu-card-title">OPPO Research Institute</p>
    <p><strong>Role:</strong> Research Intern</p>
    <p>Worked on robot motion development and debugging. The robot I helped build and tune was showcased in a live performance at the OPPO annual meeting.</p>
    <div class="photo-grid">
      <figure>
        <img src="images/image/oppo_hezhao1_web.jpg" alt="Group photo with the team at OPPO Research Institute">
      </figure>
      <figure>
        <img src="images/image/oppo_hezhao2_web.jpg" alt="Group photo with the team at OPPO Research Institute">
      </figure>
    </div>
    <p class="media-note">With the team at the OPPO Research Institute.</p>
  </div>
</div> -->


<span class='anchor' id='-academic-projects'></span>
# ⚙️ Academic Projects

<div class='paper-box'><div class='paper-box-image'><div><img src='images/Academic_Projects/kindergarten.gif' alt="Smart Campus Personnel Safety System Demo" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<span class="proj-title">Smart Campus Personnel Safety Behavior Analysis and Early Warning System</span>

<p style="text-align: justify;">
This project responds to the growing need for digital and intelligent upgrades in campus administration. It delivers three capabilities: intruder detection along campus fences, an alert system for dangerous student behaviors, and a classroom management system that monitors attention and abnormal activity during class.
</p>

- *Deployed at Qingya Kindergarten, Huaiyin District, Jinan, China.*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Academic_Projects/bird.gif' alt="Intelligent Bird Repellent System Demo" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<span class="proj-title">Intelligent Bird Repellent System</span>

<p style="text-align: justify;">
Birds perching and nesting on transmission towers cause both bird electrocution and costly power grid trips. To mitigate these hazards proactively, we developed a laser-based bird repellent system that detects and tracks birds in real time with <strong>YOLOv5 + DeepSORT</strong>.
</p>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/Academic_Projects/Rebar.jpg' alt="Rebar Tensile Strength Qualification Detection Demo" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<span class="proj-title">Image Recognition-Based System for Rebar Tensile Strength Qualification</span>

<p style="text-align: justify;">
This system combines image processing and deep learning to automatically assess the quality of steel rebar after tensile testing. By making qualification decisions precise and repeatable, it reduces human error, accelerates material verification, and ultimately contributes to safer and more reliable infrastructure.
</p>

</div>
</div>


# 🏅 Honors and Awards
- [*2025.10*]&nbsp;&nbsp;&nbsp;&nbsp;3rd Place, Mecha Challenge (Robot Dance Championship), IROS 2025.
- [*2025.06*]&nbsp;&nbsp;&nbsp;&nbsp;2nd Place, APTOS 2025 Big Data Challenge.
- [*2025.05*]&nbsp;&nbsp;&nbsp;&nbsp;May Fourth Youth Science Award, Shandong University (Top 1%).
- [*2024.11*]&nbsp;&nbsp;&nbsp;&nbsp;National 2nd Prize, China Graduate Mathematical Modeling Contest (Huawei Cup).
- [*2023.06*]&nbsp;&nbsp;&nbsp;&nbsp;1st Place, SoccerNet Action Spotting Challenge, CVSports Workshop at CVPR 2023.
- [*2023.06*]&nbsp;&nbsp;&nbsp;&nbsp;Outstanding Undergraduate Graduate of Shandong Province.
- [*2022.01*]&nbsp;&nbsp;&nbsp;&nbsp;1st Prize, Shandong Province Undergraduate Science and Technology Innovation Competition.
- [*2021.11*]&nbsp;&nbsp;&nbsp;&nbsp;First-Class Academic Scholarship, Shandong University.

<div class="photo-grid photo-grid--strip">
  <figure>
    <a href="images/image/cert_iros_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/cert_iros_web.jpg" alt="Bronze medal certificate, Mecha Challenge at IROS 2025">
    </a>
    <figcaption>🥉 3rd Place<br>Mecha Challenge, IROS 2025</figcaption>
  </figure>
  <figure>
    <a href="images/image/award_54_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/award_54_web.jpg" alt="Receiving the May Fourth Youth Science Award at Shandong University">
    </a>
    <figcaption>🏅 May Fourth Youth Science Award<br>Shandong University</figcaption>
  </figure>
  <figure>
    <a href="images/image/cert_huawei_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/cert_huawei_web.jpg" alt="National Second Prize certificate, China Graduate Mathematical Modeling Contest">
    </a>
    <figcaption>🏅 National 2nd Prize<br>Huawei Cup</figcaption>
  </figure>
  <figure>
    <a href="images/image/cert_cvpr_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/cert_cvpr_web.jpg" alt="First prize certificate, SoccerNet Action Spotting Challenge at CVPR 2023">
    </a>
    <figcaption>🏆 1st Place<br>SoccerNet Action Spotting, CVPR 2023</figcaption>
  </figure>
  <figure>
    <a href="images/image/cert_sdgrad_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/cert_sdgrad_web.jpg" alt="Outstanding Undergraduate Graduate of Shandong Province certificate">
    </a>
    <figcaption>🏅 Outstanding Graduate<br>Shandong Province, 2023</figcaption>
  </figure>
</div>

<!-- <p class="media-note">Click a certificate to view it in full size.</p> -->

# 📖 Education

<div class="edu-card">
  <div class="edu-card-logo">
    <img src='images/Shandong_University.jpg' alt="Shandong University logo">
  </div>
  <div class="edu-card-body">
    <p class="edu-card-title">Shandong University</p>
    <p><strong>Degree:</strong> M.Eng. in Control Science and Engineering</p>
    <p><strong>Advisor:</strong> Prof. Wei Zhang</p>
    <p><strong>Thesis:</strong> Research and Implementation of Surgical Workflow Analysis Based on Query Networks and Test-Time Adaptation</p>
    <p class="edu-card-meta">Sep 2023 – Jun 2026</p>
  </div>
  <figure class="edu-card-photo">
    <a href="images/image/shuoshi_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/shuoshi_web.jpg" alt="Master's graduation photo at Shandong University">
    </a>
    <figcaption>🎓 Master's graduation, 2026.</figcaption>
  </figure>
</div>

<div class="edu-card">
  <div class="edu-card-logo">
    <img src='images/Shandong_University.jpg' alt="Shandong University logo">
  </div>
  <div class="edu-card-body">
    <p class="edu-card-title">Shandong University</p>
    <p><strong>Degree:</strong> B.Eng. in Automation</p>
    <p><strong>Advisor:</strong> Prof. Wei Zhang</p>
    <p><strong>Thesis:</strong> Human Action Recognition with Attention Mechanism</p>
    <p class="edu-card-meta">Sep 2019 – Jun 2023</p>
  </div>
  <figure class="edu-card-photo">
    <a href="images/image/benke_web.jpg" target="_blank" rel="noopener noreferrer">
      <img src="images/image/benke_web.jpg" alt="Bachelor's graduation photo at Shandong University">
    </a>
    <figcaption>🎓 Bachelor's graduation, 2023.</figcaption>
  </figure>
</div>

<br>

<div style="text-align: center;">
    <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=hB9vJPVf8Tiu-4VYekyixCzGDZbWUwu5E8TdfQqEI90&cl=ffffff&w=300"></script>
</div>

<p style="text-align: center; color: #7a8288; font-size: 0.75em; margin-top: 1.5em;">
Last updated: {{ site.time | date: "%B %Y" }}
</p>
