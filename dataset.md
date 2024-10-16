---
layout: page
title: Dataset
---

<style>
    .dataset-container {
        max-width: 900px;
        margin: 0 auto;
        padding: 30px;
    }
    .dataset-item {
        background-color: #ffffff;
        border-radius: 12px;
        padding: 25px;
        margin-bottom: 30px;
        box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .dataset-item:hover {
        transform: translateY(-5px);
        box-shadow: 0 6px 12px rgba(0,0,0,0.15);
    }
    .dataset-item h2 {
        color: #2c3e50;
        margin-top: 0;
        font-size: 1.8em;
        border-bottom: 2px solid #3498db;
        padding-bottom: 10px;
        margin-bottom: 15px;
    }
    .dataset-item p {
        color: #34495e;
        line-height: 1.8;
        font-size: 1.1em;
    }
    .dataset-item a {
        color: #3498db;
        text-decoration: none;
        font-weight: bold;
        transition: color 0.3s ease;
    }
    .dataset-item a:hover {
        color: #2980b9;
        text-decoration: underline;
    }
    .intro {
        text-align: center;
        margin-bottom: 40px;
    }
    .intro h1 {
        color: #2c3e50;
        font-size: 2.5em;
        margin-bottom: 20px;
    }
    .intro p {
        color: #34495e;
        font-size: 1.2em;
        line-height: 1.6;
        max-width: 700px;
        margin: 0 auto;
    }
</style>

<div class="dataset-container">
    <div class="intro">
        <p>Welcome to our dataset repository. Here, you'll find a collection of high-quality datasets that we've carefully collected and annotated. Please cite our paper if you use our dataset.</p>
        <p><strong>Please note:</strong> Our datasets are <em>only available for non-commercial use and academic research purposes</em>. Any commercial use is strictly prohibited.</p>
    </div>
    <div class="dataset-item">
        <h2>CBCT Dataset</h2>
        <p>This is the dataset for our 'A fully automatic AI system for tooth and alveolar bone segmentation from cone-beam CT images' paper in  Nature Communication 2022. We released partial data (50 raw data of CBCT scans collected from dental clinics) to support the results in this study with permission from respective data centers. The full datasets are protected because of privacy issues and regulation policies in hospitals. </p>
        <p><a href="https://github.com/ErdanC/Tooth-and-alveolar-bone-segmentation-from-CBCT">Download Link</a></p>
        <p><strong>Reference:</strong></p>
        <pre><code>@article{cui2022fully,
  title={A fully automatic AI system for tooth and alveolar bone segmentation from cone-beam CT images},
  author={Cui, Zhiming and Fang, Yu and Mei, Lanzhuju and Zhang, Bojun and Yu, Bo and Liu, Jiameng and Jiang, Caiwen and Sun, Yuhang and Ma, Lei and Huang, Jiawei and others},
  journal={Nature communications},
  volume={13},
  number={1},
  pages={2096},
  year={2022},
  publisher={Nature Publishing Group UK London}
}</code></pre>
    </div>
    <div class="dataset-item">
        <h2>CephAdoAdu Dataset</h2>
        <p>We collected a new benchmark dataset, named CephAdoAdu, with both adolescent and adult cases, distinguishing it from existing datasets that solely consist of either adolescent or most adult cases. CephAdoAdu has a total of 1000 (500 adult cases, 500 adolescent cases) cephalometric X-ray images, acquired from eight clinical centers. Every cephalometric image underwent manual annotations to mark 10 typical landmarks, by an experienced dental radiologist with over ten years of expertise.</p>
        <p><a href="https://github.com/ShanghaiTech-IMPACT/CeLDA/">Download Link</a></p>
        <p><strong>Reference:</strong></p>
        <pre><code>@inproceedings{wu2024cephalometric,
  title={Cephalometric Landmark Detection across Ages with Prototypical Network},
  author={Wu, Han and Wang, Chong and Mei, Lanzhuju and Yang, Tong and Zhu, Min and Shen, Dinggang and Cui, Zhiming},
  booktitle={International Conference on Medical Image Computing and Computer-Assisted Intervention},
  pages={155--165},
  year={2024},
  organization={Springer}
}</code></pre>
    </div>
</div>
