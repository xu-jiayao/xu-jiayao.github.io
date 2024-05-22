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
I obtained my Ph.D. degree from Hosei University in March 2024 and my M.S. degree in September 2020. 

My **research interest** lies in _**Image Codec design**_ based on _**Compressive Sensing**_, which encompasses _**Hardware Implementation**_ and _**Deep Learning**_. 

Throughout my doctoral and master's studies, I have authored 10 papers, most of which have been published in leading conferences and journals in the fields of image processing and hardware implementation, including **TMM, CVM, MMM, ISCAS, DCC, ICIP, IJCNN**, among others. 

I possess a strong ability for **self-directed learning** and have **independently acquired knowledge** in areas relevant to my research topic during my graduate studies, as well as in iOS application development during my undergraduate studies.

I am currently actively seeking post-doctoral or researcher opportunities and aspire to join a growth-oriented team where I can make meaningful contributions to advancement and development. 

# 🎥 About Compressive Sensing and Image Codec
-  **Image Codec (Encoder & Decoder)**
   
   Similar to other data compression and feature extraction techniques, the aim of image codecs is to reduce image redundancies, thereby necessitating fewer bits to convey the entire image information, thus conserving storage space while preserving quality.
   
   Compression methods utilized in image codecs can be categorized into two main groups: lossy compression and lossless compression.
   Both categories seek to exploit similarities among image blocks to diminish the volume of the original data, thereby enhancing compression ratios.
   
   In convolutional codecs, such as HEVC and JPEG, the decoder performs the inverse operations of the encoder, typically requiring less computational power. The specific details related to convolutional codecs are as follows:

   ([high resolution version of Fig.1](/images/research/convolutional codec frameworks.pdf))
   
  <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/images/research/convolutional codec frameworks.bmp">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Figure 1. The convolutional codecs framework.</div>
  </center>
<br> 
   
 
-  **Compressive Sensing (CS)**

   As a leading field in representing low-dimensional structured data, Compressive Sensing (CS) emerges as a groundbreaking theory in signal sampling.
   It transcends the constraints of the conventional Nyquist sampling theorem by capitalizing on data sparsity to enable downsampling, thereby reducing hardware demands in analog-to-digital (A/D) processing.

   ([high resolution version of Fig.2](/images/research/compressive sensing framework.pdf))
   
  <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/images/research/compressive sensing framework.bmp">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Figure 2. The Compressive Sensing framework. <br> 
      It offers cost-effective sampling compared to convolutional codecs but encounters two main challenges: inadequate compression ratios, measured in bits per pixel (bpp), and difficulties in real-time processing due to the reconstruction process. </div>
  </center>
   <br> 

   In CS, sampling and compression involve straightforward linear projections, shifting the computational complexity to the reconstruction, similar to the role of decoders in convolutional image codecs. 
   
   Down-sampling is achieved by reducing the signal's dimensionality, and the compression ratio of CS represents the dimensional ratio between the original and compressed signals.
   **However, the compression ratio, in terms of bits per pixel (bpp), is still not satisfied.**
  
   This process of sampling and compression, which involves hardware devices, is typically implemented through software simulation. The details of the simulation are as follows:
   
   ([high resolution version of Fig.3](/images/research/sampling.pdf))

   <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/images/research/sampling.bmp">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Figure 3. The sampling and compression process in CS. </div>
  </center>
  <br> 
   
  **On the other hand, reconstruction is an NP-hard problem, making real-time processing challenging, thus becoming a primary bottleneck in CS applications.**
   
   Two conditions are essential to guarantee successful reconstruction. The first is the sparsity of the original signal. Since image signals are dense, a transform matrix is introduced to sparsify the image signal. The second condition is the incoherence between the transform matrix and the measurement matrix. 
   
<!---   The reconstruction theory, reconstruction process, and the relationship among parameters used in reconstruction are as follows:
   
   ([high resolution version of Fig.4](/images/research/reconstruction problem.pdf))

   <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/images/research/reconstruction problem.BMP">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Figure 4. The reconstruction issue description. </div>
  </center>
  <br> 

  ([high resolution version of Fig.5](/images/research/reconstruction process.pdf))

   <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/images/research/reconstruction process.bmp">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Figure 5. The reconstruction process. </div>
  </center>
  <br> 

  ([high resolution version of Fig.6](/images/research/parameter relation.pdf))

   <center>
    <img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
    src="/images/research/parameter relation.bmp">
    <br>
    <div style="color:orange; border-bottom: 1px solid #d9d9d9;
    display: inline-block;
    color: #999;
    padding: 2px;">Figure 6. The relationship among parameters used in the reconstruction. </div>
  </center>
  <br>  ---!>


# 📝 Publications 

- `TMM` [Compressive Sensing Based Image Codec With Partial Pre-Calculation](https://ieeexplore.ieee.org/abstract/document/10297548)
**Jiayao Xu**, Jian Yang, Fuma Kimishima, Ittetsu Taniguchi, Jinjia Zhou


- `MMM` [Real-time FPGA Design for OMP Targeting 8K image Reconstruction](https://link.springer.com/chapter/10.1007/978-3-030-98358-1_41)
**Jiayao Xu**, Chen Fu, Zhiqiang Zhang, Jinjia Zhou

- `ISCAS` [An 81.92Gpixels/s Fast Reconstruction of Images from Compressively Sensed Measurements](https://ieeexplore.ieee.org/abstract/document/9937930)
**Jiayao Xu**, Pham Do Kim Chi, Chen Fu, Jinjia Zhou

- `ICVIP` [High-speed Compressed Sensing Reconstruction using Zigzag Ordering based Parallel Processing](https://dl.acm.org/doi/abs/10.1145/3447450.3447489)
**Jiayao Xu**, Jirayu Peetakul, Muchen Li, Jinjia Zhou

- `Peer Review` [Plug-and-Play Adaptive Block Compressive Sensing using Edge-Detection on the Compressed Domain]
**Jiayao Xu**, Yibo Fan, Jinjia Zhou

- `CVM, ACCEPT` [JVCSR+: Adaptively Learned Video Compressive Sensing Reconstruction with Joint In-loop Reference Enhancement and Out-loop Super-resolution] 
Jian Yang, **Jiayao Xu**, Jinjia Zhou

- `DCC` [Zigzag Ordered Walsh Matrix for Compressed Sensing Image Sensor](https://ieeexplore.ieee.org/abstract/document/10125342)
Jinyao Zhou, **Jiayao Xu**, Jirayu Peetakul, Jinjia Zhou

- `ICIP` [Dynamic Unilateral Dual Learning for Text-to-Image Synthesis](https://ieeexplore.ieee.org/abstract/document/10223128)
Zhiqiang Zhang, **Jiayao Xu**, Ryugo Morita, Wenxin Yu, Jinjia Zhou

- `IJCNN, ACCEPT` [High Frequency Feature Distillation Network for Compressive Sensing Reconstruction]
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

• Introduction:

Provide on-campus student services such as checking lecture schedules, accessing library book collection information, verifying campus card balances, and processing recharges.

• Responsibility:
  
1. Contributed to API design and revised API documentation to enhance comprehension and utilization by the development team.

2. Conducted a refactoring of the existing application, employing Git version control to facilitate code collaboration and project management. Utilized various design patterns to reduce coupling and enhance code maintainability.

3. Developed and integrated functionality for library and login modules, implementing rigorous testing methods to validate code accuracy and reinforce system stability.

4. Orchestrated the implementation of the network layer, encapsulating data packets in JSON format. Collaborated closely with the backend team to conduct comprehensive testing of the network layer, ensuring seamless communication with backend services and making necessary adjustments to meet project requirements.


<img src="/images/iswust1.jpg" width="300" >
<img src="/images/iswust2.png" width="300" >



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



