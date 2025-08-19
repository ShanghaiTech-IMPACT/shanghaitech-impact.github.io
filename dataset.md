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
        border-bottom: 2px solid #2c3e50;;
        padding-bottom: 10px;
        margin-bottom: 15px;
    }
    .dataset-item p {
        color: #34495e;
        line-height: 1.8;
        font-size: 1.1em;
    }
    .dataset-item a {
        color: #2c3e50;;
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
        margin-bottom: 50px;
        background: #ffffff;
        color: #2c3e50;
        padding: 40px 30px;
        border-radius: 20px;
        box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        border: 1px solid #e8e8e8;
    }
    .intro h1 {
        color: #2c3e50;
        font-size: 2.8em;
        margin-bottom: 20px;
        font-weight: 300;
        text-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    .intro .welcome-text {
        color: #34495e;
        font-size: 1.3em;
        line-height: 1.7;
        max-width: 750px;
        margin: 0 auto 30px auto;
        font-weight: 300;
    }
    .notice-box {
        background: #fff3cd;
        border: 2px solid #ffc107;
        border-radius: 15px;
        padding: 25px;
        margin-top: 30px;
    }
    .notice-title {
        color: #856404;
        font-size: 1.4em;
        font-weight: 600;
        margin-bottom: 15px;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }
    .notice-title::before {
        content: "⚠️";
        font-size: 1.2em;
    }
    .notice-content {
        color: #856404;
        text-align: left;
        line-height: 1.8;
        font-size: 1.1em;
    }
    .notice-content ul {
        margin: 0;
        padding-left: 20px;
    }
    .notice-content li {
        margin-bottom: 12px;
        list-style-type: none;
        position: relative;
    }
    .notice-content li::before {
        content: "•";
        color: #ffc107;
        font-weight: bold;
        position: absolute;
        left: -15px;
    }
    .highlight-text {
        background: #ffd54f;
        padding: 2px 6px;
        border-radius: 4px;
        font-weight: 600;
        color: #5d4037;
    }
    .notice-content a {
        color: #2980b9;
        text-decoration: none;
        font-weight: 600;
        background: rgba(41, 128, 185, 0.1);
        padding: 3px 8px;
        border-radius: 6px;
        border: 1px solid rgba(41, 128, 185, 0.3);
        transition: all 0.3s ease;
        display: inline-block;
        margin: 0 2px;
    }
    .notice-content a:hover {
        background: #2980b9;
        color: white;
        border-color: #2980b9;
        transform: translateY(-1px);
        box-shadow: 0 2px 4px rgba(41, 128, 185, 0.3);
    }
    .notice-content a::before {
        content: "📄 ";
        margin-right: 4px;
    }
</style>

<div class="dataset-container">
    <div class="intro">
        <p class="welcome-text">
            Welcome to our dataset repository. Here, you'll find a collection of high-quality datasets that we've carefully collected and annotated. Please cite our paper if you use our dataset.
        </p>
        <div class="notice-box">
            <div class="notice-title">Important Notice</div>
            <div class="notice-content">
                <ul>
                    <li>Our datasets are <span class="highlight-text">available only for non-commercial and academic research purposes</span>. Any form of commercial use is strictly prohibited.</li>
                    <li>Access to all datasets is granted through an application and review process. To request access, please complete the <a href="./assets/data-request-form.pdf">Data Access Application Form</a> and email it to the first author of the corresponding paper and Dr. Zhiming Cui, while also cc your supervisor. Upon approval, you will receive the download link.</li>
                </ul>
            </div>
        </div>
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
    <div class="dataset-item">
        <h2>Tooth Alignment Dataset</h2>
        <p>We acquire 2,224 CBCT scans from Shanghai NinthPeople’s Hospital under consistent acquisition parameters (100 kVsource voltage, 0.3 mm voxel size, 468 × 468 × 250 resolution). Eachscan undergoes rigid registration to align it to a standardized jawcoordinate system for uniform orientation and field of view, and weapply stringent quality control to remove scans with metal or motionartifacts and incomplete dentition coverage. The resulting dataset comprises1,955 clinically validated high-quality sets of 3D tooth models.</p>
        <p><a href="https://github.com/ShanghaiTech-IMPACT/CLIK-Diffusion">Download Link</a></p>
        <p><strong>Reference:</strong></p>
        <pre><code>@article{DOU2025103746,
title = {CLIK-Diffusion: Clinical Knowledge-informed Diffusion Model for Tooth Alignment},
journal = {Medical Image Analysis},
volume = {106},
pages = {103746},
year = {2025},
issn = {1361-8415},
doi = {https://doi.org/10.1016/j.media.2025.103746},
url = {https://www.sciencedirect.com/science/article/pii/S1361841525002932},
author = {Yulong Dou and Han Wu and Changjian Li and Chen Wang and Tong Yang and Min Zhu and Dinggang Shen and Zhiming Cui}
}</code></pre>
    </div>
</div>
