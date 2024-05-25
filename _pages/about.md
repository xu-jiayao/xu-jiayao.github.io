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

# 🙋‍♀️ Profile 
I obtained my Ph.D. degree from Hosei University in March 2024 and my M.S. degree in September 2020, under the supervision of [Prof. Jinjia Zhou](https://www.zhou-lab.info/jinjia-zhou).

My **research interest** lies in _**Image Codec design**_ based on _**Compressive Sensing**_, which encompasses _**Hardware Implementation**_ and _**Deep Learning**_. 

Throughout my doctoral and master's studies, I have authored **10 papers**, most of which have been published in leading conferences and journals in the fields of image processing and hardware implementation, including **TMM, CVM, MMM, ISCAS, DCC, ICIP, IJCNN**, among others. 

I possess a strong ability for **self-directed learning** and have **independently acquired knowledge** in areas relevant to my research topic during my graduate studies, as well as in iOS application development during my undergraduate studies.

I am currently actively seeking post-doctoral or researcher opportunities and aspire to join a growth-oriented team where I can make meaningful contributions to advancement and development. 

# 🔥 News
- *2024.03*: 🎉 One paper is accepted by **IJCNN oral** 2024!
- *2024.01*: 🎉 One paper is accepted by **CVM journal**!
- *2023.10*, 🎉 Keynote speech on Compressive Sensing at Institut National des Sciences Appliquées de Rennes, INSA de Rennes.
- *2023.10*: 🎉 One paper is accepted by **TMM**!
- *2023.06*: 🎉 One paper is accepted by **ICIP oral** 2023!
- *2023.06*: 🎉 Become a reviewer for **ECAI 2023**!
- *2023.02*: 🎉 One paper is accepted by **DCC poster** 2023!
- *2022.09*, 🎉 Initiate recurring seminars with Fudan University and Zhejiang University.
- *2022.08*, 🎉 Keynote speech on Compressive Sensing at Osaka University.
- *2022.06*, 🎉 One paper is accepted by **MMM oral** 2022!
- *2022.05*, 🎉 One paper is accepted by **ISCAS oral** 2022!


# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TMM 2023</div><img src='images/projects/TMM_methods.PNG' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<font size = 4><u><b>Compressive Sensing Based Image Codec With Partial Pre-Calculation</b></u></font>

**Jiayao Xu**, Jian Yang, Fuma Kimishima, Ittetsu Taniguchi, Jinjia Zhou

<font color=darkred> IEEE Transaction on Multimedia, 2023</font>


<font color=darkred> (<b>IF = 8.182</b>, Top Journal in Image Processing) </font>

**Key Idea**: 

Break the current codec framework and analyze the data characteristics within each process. Utilize the sparsity of matrices and processed data to introduce an innovative codec framework based on Compressive Sensing.

[**Paper**](https://ieeexplore.ieee.org/abstract/document/10297548)
/
[**Project**](https://xu-jiayao.github.io/projects/TMM/) 

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MMM 2022</div><img src='images/projects/MMM_methods.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<font size = 4><u><b>Real-time FPGA Design for OMP Targeting 8K image Reconstruction</b></u></font>

**Jiayao Xu**, Chen Fu, Zhiqiang Zhang, Jinjia Zhou

<font color=darkred>28th International Conference on Multimedia Modeling (MMM), 2022</font>

**Key Idea**: 

Due to hardware limitations in sampling, we begin our work with a deterministic matrix. 
We utilize the sparsity of the chosen sensing matrix to streamline calculations in each iteration of reconstruction.

[**Paper**](https://link.springer.com/chapter/10.1007/978-3-030-98358-1_41)
<!-- /
[**Project**](https://xu-jiayao.github.io/projects/MMM/)  -->

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ISCAS 2022</div><img src='images/projects/ISCAS_methods.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<font size = 4><u><b>An 81.92Gpixels/s Fast Reconstruction of Images from Compressively Sensed Measurements</b></u></font>

**Jiayao Xu**, Pham Do Kim Chi, Chen Fu, Jinjia Zhou

<font color=darkred>The IEEE International Symposium on Circuits and Systems (ISCAS), 2022</font>

**Key Idea**: 

We employ a sparse sensing matrix composed mainly of zero-vectors, resulting in an invertible full-rank matrix after removing these vectors, enabling the replacement of the iteration-based reconstruction procedure with a single matrix multiplication.

[**Paper**](https://ieeexplore.ieee.org/abstract/document/9937930)
<!-- /
[**Project**](https://xu-jiayao.github.io/projects/ISCAS/)  -->

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Peer Review</div><img src='images/projects/CVM_methods.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<font size = 4><u><b>Plug-and-Play Adaptive Block Compressive Sensing using Edge-Detection on the Compressed Domain</b></u></font>

**Jiayao Xu**, Yibo Fan, Jinjia Zhou

**Key Idea**: 

We recognize the correlation between edge detection and Compressive Sensing sampling, proposing an adaptive method that directly processes sampled data, thereby cutting time and hardware costs.


<!-- [**Project**](https://xu-jiayao.github.io/projects/CVM/) -->

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICVIP 2020</div><img src='images/projects/ICVIP_methods.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<font size = 4><u><b>High-speed Compressed Sensing Reconstruction using Zigzag Ordering based Parallel Processing</b></u></font>

**Jiayao Xu**, Jirayu Peetakul, Muchen Li, Jinjia Zhou

<font color=darkred>International Conference on Video and Image Processing (ICVIP), 2020</font>

**Key Idea**: 

We implement Zigzag ordering-based parallelism in the reconstruction process to ensure efficient calculations between blocks during parallel reconstruction.


[**Paper**](https://dl.acm.org/doi/abs/10.1145/3447450.3447489)
<!-- /
[**Project**](https://xu-jiayao.github.io/projects/ICVIP/) -->

</div>
</div>

- `CVM, ACCEPT` JVCSR+: Adaptively Learned Video Compressive Sensing Reconstruction with Joint In-loop Reference Enhancement and Out-loop Super-resolution
Jian Yang, **Jiayao Xu**, Jinjia Zhou

- `DCC` [Zigzag Ordered Walsh Matrix for Compressed Sensing Image Sensor](https://ieeexplore.ieee.org/abstract/document/10125342)
Jinyao Zhou, **Jiayao Xu**, Jirayu Peetakul, Jinjia Zhou

- `ICIP` [Dynamic Unilateral Dual Learning for Text-to-Image Synthesis](https://ieeexplore.ieee.org/abstract/document/10223128)
Zhiqiang Zhang, **Jiayao Xu**, Ryugo Morita, Wenxin Yu, Jinjia Zhou

- `IJCNN, ACCEPT` High Frequency Feature Distillation Network for Compressive Sensing Reconstruction
Fuma Kimishima, **Jiayao Xu**, Jinjia Zhou

- `MMSP` [Optimizing CABAC architecture with prediction based context model prefetching](https://ieeexplore.ieee.org/abstract/document/9949499)
Chen Fu, Heming Sun, **Jiayao Xu**, Zhiqiang Zhang, Jinjia Zhou


# 🔥 Skills
• **Languages:** English - TOEIC(845/990), Japanese - JLPT N2(120/180), Mandarin - Native speaker

• **Programming Languages:** Python, C/C++, MATLAB, Verilog , Objective-C

• **Software Development:** Object-Oriented Programming (OOP), Design Patterns, Team Collaboration

• **Platform:** Visual Studio Code, MATLAB, Modelsim, Vivado, XCode, Wireshark, Git version control

• **OS (environment setting and system maintenance):** Windows, Centos 7, Ubuntu 18, macOS

# 👩‍💻 iOS Project
**Name**: iSWUST (i西科) 

**Supported users**: 3,000+ Active Users 

**Laboratory**: Mobile Web Laboratory (移动互联网实验室)

**Work duration**: Sep.2015 – Mar.2017

**Release Time**: December 4th, 2016

**Current status**: out of service.

**Introduction**:

Provide on-campus student services such as checking lecture schedules, accessing library book collection information, verifying campus card balances, and processing recharges.

**Responsibility**:
  
1. Contributed to API design and revised API documentation to enhance comprehension and utilization by the development team.

2. Conducted a refactoring of the existing application, employing Git version control to facilitate code collaboration and project management. Utilized various design patterns to reduce coupling and enhance code maintainability.

3. Developed and integrated functionality for library and login modules, implementing rigorous testing methods to validate code accuracy and reinforce system stability.

4. Orchestrated the implementation of the network layer, encapsulating data packets in JSON format. Collaborated closely with the backend team to conduct comprehensive testing of the network layer, ensuring seamless communication with backend services and making necessary adjustments to meet project requirements.

<!--- <center>
<img src="/images/iswust1.jpg" width="300" >  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/images/iswust2.png" width="300" >
</center> -->


# 📖 Educations
- *2020.09 - 2024.03*, Ph.D, Hosei University, Tokyo, Japan.
- *2018.09 - 2020.09*, Master, Hosei University, Tokyo, Japan.
- *2014.09 - 2018.06*, Bachelor, Southwest University of Science and Technology, Sichuan, China.

# 💬 Invited Talks
- *2023.10*, Compressive Sensing Based Image Codec With Partial Pre-Calculation talk in Institut National des Sciences Appliquées de Rennes, INSA de Rennes.
- *2022.09 - 2024.03*, Regular seminar with Fudan University and Zhejiang University for Image Compression using Compressive Sensing.
- *2022.08*, Compressive Sensing Seminar with Osaka Univerisity.
- *2022.06*, Real-time hardware design for Compressive Sensing reconstruction talk, MMM 2022.
- *2022.05*, a hardware design reaches 81.92 GPixel/s for Compressive Sensing reconstruction talk, ISCAS 2022.
- *2020.12*, Parallel reconstruction design for Compressive Sensing reconstruction talk, ICVIP 2020.

# 🎖 Honors and Awards
- *2020-2023* Research grants from Hosei University Graduate School.
- *2020-2021* JASSO scholarship.
- *2020.12* The best presentation of all excellent presentations at the 3rd International Conference on Image and Video Processing (ICIVP 2020). 


<footer class="footer">
</footer>
