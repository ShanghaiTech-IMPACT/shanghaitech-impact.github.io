---
layout: page
title: People
---

<style>
    .rounded-image {
        width: 200px;
        height: 200px;
        border-radius: 50%;
        border: 5px solid #e0e0e0;
        object-fit: cover; 
        object-position: center;
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .rounded-image:hover {
        transform: scale(1.05);
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    @media (max-width: 600px) {
        .rounded-image {
            width: 120px;  
            height: 120px;  
            border-width: 3px;
        }
    }

    table.people {
        width: 100%;
        table-layout: fixed;
        border-collapse: separate; 
        border-spacing: 15px;
        margin: 30px 0;
    }

    .people td {
        width: 25%;
        text-align: center;
        vertical-align: top;
        padding: 20px;
        background-color: #ffffff;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        transition: all 0.3s ease;
    }

    .people td:hover {
        transform: translateY(-5px);
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    }

    h2 {
        font-size: 2.2em;
        color: #2c3e50;
        margin: 40px 0 30px;
        border-bottom: 3px solid #3498db;
        padding-bottom: 10px;
        text-align: center;
    }

    a {
        color: #3498db;
        text-decoration: none;
        font-weight: bold;
        transition: color 0.3s ease;
    }

    a:hover {
        color: #2980b9;
    }

    .name {
        font-size: 1.2em;
        font-weight: bold;
        margin: 10px 0 5px;
    }

    .info {
        font-size: 0.9em;
        color: #7f8c8d;
    }
</style>

<h2>Gallery</h2>

<style>
    #slider {
        width: 100%;
        max-width: 800px;
        margin: 40px auto;
    }
    #image-container {
        position: relative; 
        width: 100%;  
        padding-top: 56.25%; /* 16:9 Aspect Ratio */
        height: 0;
        overflow: hidden; 
        border-radius: 10px;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }
    #image-container img {
        position: absolute; 
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        max-width: 100%;
        max-height: 100%;
        object-fit: cover; 
        opacity: 0; 
        transition: opacity 0.8s ease-in-out;
    }
    #image-container img.active {
        opacity: 1; 
    }
    .slider-nav {
        display: flex;
        justify-content: center;
        margin-top: 20px;
    }
    .slider-nav button {
        background-color: #3498db;
        color: white;
        border: none;
        padding: 10px 20px;
        margin: 0 10px;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }
    .slider-nav button:hover {
        background-color: #2980b9;
    }
</style>

<div id="slider">
    <div id="image-container">
        <img src="/assets/img/Gallery/20240328.jpg" alt="Gallery Image 1">
        <img src="/assets/img/Gallery/20230919_0.jpg" alt="Gallery Image 2">
        <img src="/assets/img/Gallery/20230617_2.jpg" alt="Gallery Image 3">
        <img src="/assets/img/Gallery/UMI2024.png" alt="Gallery Image 4">
        <img src="/assets/img/Gallery/MLMI2024.jpg" alt="Gallery Image 5">
    </div>
    <div class="slider-nav">
        <button onclick="prevSlide()">Previous</button>
        <button onclick="nextSlide()">Next</button>
    </div>
</div>

<script>
    var slider = document.getElementById("slider");
    var imageContainer = document.getElementById("image-container");
    var images = imageContainer.getElementsByTagName("img");
    var index = 0;
    var speed = 5000; // 5 seconds

    function showSlide(n) {
        images[index].classList.remove("active");
        index = (n + images.length) % images.length;
        images[index].classList.add("active");
    }

    function nextSlide() {
        showSlide(index + 1);
    }

    function prevSlide() {
        showSlide(index - 1);
    }

    function autoSlide() {
        nextSlide();
        setTimeout(autoSlide, speed);
    }

    // Start the slideshow
    showSlide(0);
    setTimeout(autoSlide, speed);
</script>

<h2>Ph.D. Students</h2>

<table class="people" id="phd-students">
    <tr>
        <td>
            <img src="/assets/img/people/HanWu.png" class="rounded-image" alt="Han Wu">
            <div class="name"><a href="http://hanwu.website/">Han Wu</a></div>
            <div class="info">Ph.D. since 2022<br>B.E. WUT</div>
            <!-- <div class="info">(with Prof. Dinggang Shen)</div> -->
        </td>
        <td>
            <img src="/assets/img/people/ZhentaoLiu.jpg" class="rounded-image" alt="Zhentao Liu">
            <div class="name"><a href="https://zhentao-liu.github.io/">Zhentao Liu</a></div>
            <div class="info">Ph.D. since 2022<br>B.E. NBU</div>
        </td>
        <td>
            <img src="/assets/img/people/RuochenPi.jpg" class="rounded-image" alt="Ruochen Pi">
            <div class="name">Ruochen Pi</div>
            <div class="info">Eng.D. since 2024<br>M.S. USYD, B.E. SHNU</div>
        </td>
        <td></td>
    </tr>
</table>

<h2>Graduate Students</h2>

<table class="people" id="graduate-students">
    <tr>
        <td>
            <img src="/assets/img/people/HaoshenWang.jpg" class="rounded-image" alt="Haoshen Wang">
            <div class="name">Haoshen Wang</div>
            <div class="info">M.S. since 2022<br>B.E. DUT</div>
        </td>
        <td>
            <img src="/assets/img/people/YulongDou.jpg" class="rounded-image" alt="Yulong Dou">
            <div class="name"><a href="https://douyl.github.io/">Yulong Dou</a></div>
            <div class="info">M.S. since 2023<br>B.E. ShanghaiTech</div>
        </td>
        <td>
            <img src="/assets/img/people/ChenfanXu.png" class="rounded-image" alt="Chenfan Xu">
            <div class="name">Chenfan Xu</div>
            <div class="info">M.S. since 2023<br>B.E. SHU</div>
        </td>
        <td>
            <img src="/assets/img/people/XingyueWang.jpg" class="rounded-image" alt="Xingyue Wang">
            <div class="name">Xingyue Wang</div>
            <div class="info">M.S. since 2023<br>B.E. TMU & TJU</div>
        </td>
    </tr>
    <tr>
        <td>
            <img src="/assets/img/people/ZhenyuTao.jpg" class="rounded-image" alt="Zhenyu Tao">
            <div class="name">Zhenyu Tao</div>
            <div class="info">M.Eng. since 2023<br>B.E. HFUT</div>
        </td>
        <td>
            <img src="/assets/img/people/TaoLuo.jpg" class="rounded-image" alt="Tao Luo">
            <div class="name">Tao Luo</div>
            <div class="info">M.S. since 2024<br>B.E. SWU</div>
        </td>
        <td>
            <img src="/assets/img/people/ZihuanLi.jpg" class="rounded-image" alt="Zihuan Li">
            <div class="name">Zihuan Li</div>
            <div class="info">M.S. since 2024<br>B.E. HIT</div>
        </td>
        <td>
            <img src="/assets/img/people/ZhihaoZhang.jpg" class="rounded-image" alt="Zhihao Zhang">
            <div class="name">Zhihao Zhang</div>
            <div class="info">M.S. since 2024<br>B.E. NJUPT</div>
        </td>
    </tr>
    <tr>
        <td>
            <img src="/assets/img/people/LuqiYang.jpg" class="rounded-image" alt="Luqi Yang">
            <div class="name">Luqi Yang</div>
            <div class="info">M.Eng. since 2024<br>B.E. DUT</div>
        </td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
</table>

<h2>Visiting Students</h2>

<table class="people" id="visiting-students">
    <tr>
        <td>
            <img src="/assets/img/people/JiaminWu.png" class="rounded-image" alt="Jiamin Wu">
            <div class="name">Jiamin Wu</div>
            <div class="info">Ph.D. from HKU</div>
        </td>
        <td>
            <img src="/assets/img/people/QingyaoLuo.jpg" class="rounded-image" alt="Qingyao Luo">
            <div class="name">Qingyao Luo</div>
            <div class="info">M.S. from NEU</div>
        </td>
        <td>
            <img src="/assets/img/people/ZichenZhang.jpg" class="rounded-image" alt="Zichen Zhang">
            <div class="name">Zichen Zhang</div>
            <div class="info">M.S. from TUM</div>
        </td>
        <td></td>
    </tr>
</table>

<h2>Undergraduate Students</h2>

<table class="people" id="undergraduate-students">
    <tr>
        <td>
            <img src="/assets/img/people/SiyuChen.jpeg" class="rounded-image" alt="Siyu Chen">
            <div class="name">Siyu Chen</div>
            <div class="info">Class 2021</div>
        </td>
        <td>
            <img src="/assets/img/people/WeiJia.png" class="rounded-image" alt="Wei Jia">
            <div class="name">Wei Jia</div>
            <div class="info">Class 2022</div>
        </td>
        <td>
            <img src="/assets/img/people/JinzeWu.jpg" class="rounded-image" alt="Jinze Wu">
            <div class="name">Jinze Wu</div>
            <div class="info">Class 2022</div>
        </td>
        <td>
            <img src="/assets/img/people/GuoChen.jpg" class="rounded-image" alt="Guo Chen">
            <div class="name">Guo Chen</div>
            <div class="info">Class 2022</div>
        </td>
    </tr>
</table>

<!-- 
<h2>Alumni</h2>

<table class="people" id="alumni">
    <tr>
        <td>
            <img src="/assets/img/people/HaoshenWang.jpg" class="rounded-image" alt="Haoshen Wang">
            <div class="name">Haoshen Wang</div>
            <div class="info">M.S. 2022.09 - 2024.06</div>
            <div class="info">B.E. DUT</div>
            <div class="info">Current: PhD @ HKPolyU</div>
        </td>
        <td>
            <img src="/assets/img/people/QingyaoLuo.jpg" class="rounded-image" alt="Qingyao Luo">
            <div class="name">Qingyao Luo</div>
            <div class="info">Visiting M.S. from NEU</div>
            <div class="info">2023.07 - 2024.10</div>
        </td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
</table> 
 -->
