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


I am **Xiangtai** and I work as a **Research Fellow** at [MMLab@NTU](https://www.mmlab-ntu.com/) S-Lab advised by [Prof.Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/).

I obtained my PhD degree at Peking University (PKU). My PhD supervisor is [Prof.Yunhai Tong](https://scholar.google.com/citations?user=T4gqdPkAAAAJ&hl=zh-CN).
I obtained my bachelor degree at Beijing University of Posts and Telecommunications (BUPT).

🔭 I'm currently working on Pixel-Wised Scene Understanding/Vision Transformer/Video Understanding in Computer Vision. 

🔭 I am also interested at general deep learning method design and understanding with its application.
 
Previously, I did some research on Image/Video Semantic/Instance/Panoptic Segmentation as well as several related problems.

I did several works on these directions during my PhD in PKU. I am lucky mentored and also collaborate by [Dr.Kuiyuan Yang](https://scholar.google.com/citations?user=g2gAY_0AAAAJ&hl=zh-CN), [Prof.Li Zhang](http://www.robots.ox.ac.uk/~lz/), [Dr.Guangliang Cheng](https://scholar.google.com/citations?user=FToOC-wAAAAJ&hl=zh-CN), 
[Dr.Yibo Yang](https://iboing.github.io/), [Prof.Dacheng Tao](https://scholar.google.com/citations?user=RwlJNLcAAAAJ&hl=zh-CN), [Prof.Zhouchen Lin](), [Mr.Xia li](https://xialipku.github.io/), [Dr.Jiangmiao Pang](https://oceanpang.github.io/).

(video) semantic segmentation, (video) instance segmentation, (video) panoptic segmentation, panoptic segmentation with depth/part, transparent object, boundary feature learning, aerial segmentation, video object detection/tracking/segmentation，

Remote Cooperations are Welcome (lxtpku@pku.edu.cn or xiangtai.li@ntu.edu.sg).


# 🔥 News
- *2022.11*：Two paper on Video Scene Understanding is accepted by T-PAMI.
- *2022.09*：One paper on Neural Collapse is accepted by NeurIPS-2022. 
- *2022.08*： &nbsp;🎉🎉 Join the MMLab@NTU S-Lab! Our four works (Video K-Net, PanopticPartFormer, FashionFormer, and PolyphonicFormer in CVPR-22/ECCV-22) code are all released. Check out my github homepage.
- *2022.07*： &nbsp;🎉🎉 Our SFNet-Lite (extension of SFNet-ECCV20) achieve the best mIoU and speed trade-off.
on multiple driving datasets. SFNet-Lite can obtain 80.1 mIoU while running at 50 FPS, 78.8 mIoU while running at 120 FPS. [Code](https://github.com/lxtGH/SFSegNets).
- *2022.07*: &nbsp;🎉🎉 Three papers are accepted by ECCV-2022. One paper is accepted by ICIP-2022.
- *2022.07*: &nbsp;🎉🎉 Graduated From PKU. 
- *2022.03*: &nbsp;🎉🎉 Video K-Net is accepted by CVPR-2022 as oral presentation.  

# 📝 Selected Publications 

Full Publications can be found in [this](https://scholar.google.com/citations?user=FL3ReD0AAAAJ&hl=zh-CN).

\* means equal contribution.

Code can be found in [this](https://github.com/lxtGH).

## Selected Conference 

<ul>


<li><a href="https://arxiv.org/abs/2204.04655">Panoptic-PartFormer: Learning a Unified Model for Panoptic Part Segmentation</a>,  
      <strong>Xiangtai Li</strong>, Shilin Xu, Yibo Yang, Guangliang Cheng, Yunhai Tong, Dacheng Tao,
      <strong>ECCV 2022 <span style="color:red"> The first unified part-aware panoptic segmentation model</span></strong> | <a href="https://github.com/lxtGH/Panoptic-PartFormer">Code</a> </li>


<li><a href="https://arxiv.org/abs/2204.04654">Fashionformer: A Simple, Effective and Unified Baseline for Human Fashion Segmentation and Recognition</a>,  
      Shilin Xu*, <strong>Xiangtai Li*</strong>, Jingbo Wang, Guangliang Cheng, Yunhai Tong, Dacheng Tao,
      <strong>ECCV 2022 </strong> | <a href="https://github.com/xushilin1/FashionFormer">Code</a> </li>


<li><a href="https://arxiv.org/abs/2112.02582">PolyphonicFormer: Unified Query Learning for Depth-aware Video Panoptic Segmentation</a>,  
    Haobo Yuan*, <strong>Xiangtai Li*</strong>, Yibo Yang, Guangliang Cheng, Jing Zhang, Yunhai Tong, Lefei Zhang, Dacheng Tao,
      <strong>ECCV 2022 <span style="color:red"> Winner of ICCV-2021 BMTT workshop, The first unified depth aware video panoptic segmentation model</span> </strong> | <a href="https://github.com/HarborYuan/PolyphonicFormer">Code</a> </li>


<li><a href="https://arxiv.org/abs/2204.04656">Video K-Net: A Simple, Strong, and Unified Baseline for Video Segmentation</a>,  
      <strong>Xiangtai Li*</strong>, Wenwei Zhang*, Jiangmiao Pang*, Kai Chen, Guangliang Cheng, Yunhai Tong, Chen Change Loy,
      <strong>CVPR 2022 <span style="color:red">(Oral, top2%) The first unified video segmentation model and codebase for VPS, VIS, VSS</span> </strong> | <a href="https://github.com/lxtGH/Video-K-Net">Code</a> </li>


<li><a href="https://arxiv.org/abs/2103.06564">PointFlow: Flowing Semantics Through Points for Aerial Image Segmentation</a>,  
      <strong>Xiangtai Li</strong>, Hao He, Xia Li, Duo Li, Guangliang Cheng, Jianping Shi, Lubin Weng, Yunhai Tong, Zhouchen Lin,
      <strong>CVPR 2021 </strong> | <a href="https: //github.com/lxtGH/PFSegNets">Code</a> </li>

<li><a href="https://arxiv.org/abs/2103.15734">Enhanced Boundary Learning for Glass-like Object Segmentation</a>,  
      Hao He*, <strong>Xiangtai Li*</strong>, Guangliang Cheng, Jianping Shi, Yunhai Tong, Gaofeng Meng, Véronique Prinet, Lubin Weng,
      <strong>ICCV 2021 </strong> | <a href="https://github.com/hehao13/EBLNet">Code</a> </li>

<li><a href="https://arxiv.org/abs/2002.10120">Semantic Flow for Fast and Accurate Scene Parsing</a>,  
      <strong>Xiangtai Li</strong>, Ansheng You, Zhen Zhu, Houlong Zhao, Maoke Yang, Kuiyuan Yang, Yunhai Tong,
      <strong>ECCV 2020 <span style="color:red">(Oral, top2%) The first real time model over 80\% mIoU on Cityscapes test set.</span></strong> | <a href="https://github.com/lxtGH/SFSegNets">Code</a> </li>

<li><a href="https://arxiv.org/abs/2007.10035">Improving Semantic Segmentation via Decoupled Body and Edge Supervision</a>,  
      <strong>Xiangtai Li</strong>, Xia Li, Li Zhang, Guangliang Cheng, Jianping Shi, Zhouchen Lin, Shaohua Tan, Yunhai Tong,
      <strong>ECCV 2020 </strong> | <a href="https://github.com/lxtGH/DecoupleSegNets">Code</a> </li>

<li><a href="https://arxiv.org/abs/1904.01803">GFF: Gated Fully Fusion for Semantic Segmentation</a>,  
      <strong>Xiangtai Li</strong>, Houlong Zhao, Lei Han, Yunhai Tong, Kuiyuan Yang,
      <strong>AAAI 2020 <span style="color:red">(Oral)</span></strong> | <a href="https://github.com/lxtGH/DecoupleSegNets">Code</a> </li>

<li><a href="https://arxiv.org/abs/1909.06121">Dual Graph Convolutional Network for Semantic Segmentation</a>,  
      Li Zhang*, <strong>Xiangtai Li*</strong>, Anurag Arnab, Kuiyuan Yang, Yunhai Tong, Philip H. S. Torr,
      <strong>BMVC 2019 </strong> | <a href="https://github.com/lxtGH/GALD-DGCNet">Code</a> </li>

</ul>


## Journal

<ul>

<li><a href="https://arxiv.org/abs/2201.05047"> TransVOD: End-to-end Video Object Detection with Spatial-Temporal Transformers </a>,  
    Qianyu Zhou*,  <strong> Xiangtai Li* </strong>, Lu He, Yibo Yang, Guangliang Cheng, Yunhai Tong, Lizhuang Ma, Dacheng Tao,
      <strong>T-PAMI-2022</strong> | <a href="https://github.com/SJTU-LuHe/TransVOD">Code</a> </li>

<li><a href="https://arxiv.org/abs/2107.13155">Improving Video Instance Segmentation via Temporal Pyramid Routing</a>,  
      <strong>Xiangtai Li</strong>, Hao He, Yibo Yang, Henghui Ding, Kuiyuan Yang, Guangliang Cheng, Yunhai Tong, Dacheng Tao 
      <strong>T-PAMI-2022 <span style="color:red"> The first dynamic network for video scene understanding </span></strong> | <a href="https://github.com/lxtGH/TemporalPyramidRouting">Code</a> </li>

<li><a href="https://arxiv.org/abs/2011.03308">Towards Efficient Scene Understanding via Squeeze Reasoning</a>,  
      <strong>Xiangtai Li</strong>, Xia Li, Ansheng You, Li Zhang, Guangliang Cheng, Kuiyuan Yang, Yunhai Tong, Zhouchen Li,
      <strong>IEEE-TIP-2021</strong> | <a href="https://github.com/lxtGH/SFSegNets">Code</a> </li>

<li><a href="https://arxiv.org/abs/2107.13154">Global Aggregation then Local Distribution for Scene Parsing</a>,  
      <strong>Xiangtai Li*</strong>, Li Zhang*, Guangliang Cheng, Kuiyuan Yang, Yunhai Tong, Xiatian Zhu, Tao Xiang, 
      <strong>IEEE-TIP-2021</strong> | <a href="https://github.com/lxtGH/GALD-DGCNet">Code</a> </li>
</ul>

## Selected Arxiv

<ul>

<li><a href="https://arxiv.org/abs/2204.04655">Towards Robust Referring Image Segmentation</a>,  
      Jianzong Wu, <strong>Xiangtai Li</strong>, Xia Li, Henghui Ding, Yunhai Tong, Dacheng Tao,
      <strong>arxiv <span style="color:red"> The first benchmark for Robust Referring Image Segmentation</span> </strong> | <a href="../project/robust_ref_seg">Project</a> </li>


<li><a href="https://arxiv.org/abs/2206.09325"> SFNet: Faster, Accurate, and Domain Agnostic Semantic Segmentation via Semantic Flow </a>, 
      <strong>Xiangtai Li</strong>, Jiangning Zhang, Yibo Yang, Guangliang Cheng, Yunhai Tong, Kuiyuan Yang, Dacheng Tao,
      <strong>arxiv</strong> | <a href="https://github.com/lxtGH/SFSegNets">Code</a> </li>

<li><a href="https://arxiv.org/abs/2206.09325"> EATFormer: Improving Vision Transformer Inspired by Evolutionary Algorithm </a>,  
     Jiangning Zhang, <strong>Xiangtai Li</strong>, Yabiao Wang, Chengjie Wang, Yibo Yang, Yong Liu, Dacheng Tao,
      <strong>arxiv</strong> | <a href="https://https://github.com/zhangzjn/EATFormer">Code</a> </li>



<<<<<<< HEAD

=======
>>>>>>> 177b81066fefb46ce7b182a6797d7b2f35840496
<li><a href="https://arxiv.org/abs/2105.11668">BoundarySqueeze: Image Segmentation as Boundary Squeezing</a>,  
     Hao He*, <strong>Xiangtai Li*</strong>, Yibo Yang, Guangliang Cheng, Yunhai Tong, Lubin Weng, Zhouchen Lin, Shiming Xiang,
      <strong>arxiv</strong> | <a href="https://github.com/lxtGH/BSSeg">Code</a> </li>

</ul>

# 🎖 Honors and Awards
- *2021.09* National Scholarship, Ministry of Education of China in PKU (2020-2021, 2019-2020)
- *2021.06* President Scholarship of PKU (2020-2021)
- *2017, 2022* Beijing Excellent Graduates
- *2021.11* Winner of Segmenting and Tracking Every Point and Pixel: 6th Workshop on ICCV-2021 Track2 (Project Leader and First Author, 2021-10-17) 

# 📖 Educations
- *2017.09 - 2022.06*, PhD in Peking University (PKU)
- *2013.09 - 2017.06*, Bachelor in Beijing University of Posts and Telecommunications (BUPT)

# 💬 Invited Talks
- *2022.05* Invited talk on Panoptic Segmentation and Beyond in Baidu PaddleSeg Group
- *2021.12* Invited talk on Video Segmentation in DiDi Auto-Driving Group
- *2021.10* Invited talk on Aligned Segmentation HuaWei Noah Auto-Driving Group


# 💻 Internships and Professional activities
- SenseTime, mentored by Dr.Guangliang Cheng and Dr.Jianping Shi.
- JD AI (remote cooperation), mentored by Dr.Yibo Yang and Prof.Dacheng Tao.
- DeepMotion (Now Xiaomi Car), mentored by Dr.Kuiyuan Yang. 
- Conference Reviewer for CVPR, ICCV, ECCV, ICLR, AAAI, NeurIPS, ICML and Journal Reviewer For IEEE-TIP/ IEEE-TPAMI / IJCV.

# Friends and Mentored Students

Much thanks to these friends and collaborators. 

Hao He, Shilin Xu, Jianzong Wu, Haobo Yuan, Qianyu Zhou, Yangyang Xu, Ansheng You, Houlong Zhao,
Yibo Yang, Xia Li, Jingbo Wang, Jiangning Zhang, Jiangmiao Pang, Wenwei Zhang, Henghui Ding.
