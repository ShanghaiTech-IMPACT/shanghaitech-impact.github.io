---
layout: page
title: People
---


<!-- <style>
    .rounded-image {
        width: 180px;
        height: 300px;
        border-radius: 50%;
        border: 5px solid rgb(192, 192, 192);
    }
</style> -->
<style>
    .rounded-image {
        width: 180px;
        height: 250px;
        border-radius: 50%;
        border: 5px solid rgb(192, 192, 192);
        object-fit: cover;
        object-position: center;
    }
</style>

## Graduate Students

<table class="people" id="students">
    <tr>
        <td>
            <img src="/assets/img/people/HanWu.png" class="rounded-image"><br>
            <a href="http://hanwu.website/">Han Wu</a><br>
            M.Phil since 2022<br>
            B.E. WUT
        </td>
        <td>
            <img src="/assets/img/people/ZhentaoLiu.jpg" class="rounded-image"><br>
            <a href="https://github.com/Zhentao-Liu/">Zhentao Liu</a><br>
            M.Phil since 2022<br>
            B.E. NBU
        </td>
        <td>
            <img src="/assets/img/people/HaoshenWang.jpg" class="rounded-image"><br>
            Haoshen Wang<br>
            M.Phil since 2022<br>
            B.E. DUT
        </td>
    </tr>
    <tr>
        <td>
            <img src="/assets/img/people/YulongDou.jpg" class="rounded-image"><br>
            Yulong Dou<br>
            M.Phil since 2023<br>
            B.E. ShanghaiTech
        </td>
        <td>
            <img src="/assets/img/people/ChenfanXu.png" class="rounded-image"><br>
            Chenfan Xu<br>
            M.Phil since 2023<br>
            B.E. SHU
        </td>
        <td>
            <img src="/assets/img/people/XingyueWang.jpg" class="rounded-image"><br>
            Xingyue Wang<br>
            M.Phil since 2023<br>
            B.E. TMU & TJU
        </td>
    </tr>
    <tr>
        <td>
                <img src="/assets/img/people/ZhenyuTao.jpg" class="rounded-image"><br>
                Zhenyu Tao<br>
                M.Eng. since 2023<br>
                B.E. HFUT
            </td>
            <td>
                &nbsp;
            </td>
            <td>
                &nbsp;
            </td>
        </tr>
</table>






## Visiting Students
<html>
    <table class="people" id="students">
        <tr>
        <td>
                <img src="/assets/img/people/JiaminWu.png" class="rounded-image"><br>
                Jiamin Wu<br>
                Ph.D. from HKU
            </td>
            <td>
                <img src="/assets/img/people/QingyaoLuo.jpg" class="rounded-image"><br>
                Qingyao Luo<br>
                M.Phil from NEU
            </td>
            <td>
                &nbsp;
            </td>
        </tr>
    </table>
</html>

<!-- <h3>Gallery </h3> -->
## Gallery
<div id="slider">
    <div id="image-container">
        <img src="/assets/img/Gallery/20230617_0.jpg">
        <img src="/assets/img/Gallery/20230617_1.jpg">
        <img src="/assets/img/Gallery/20230617_2.jpg">
        <img src="/assets/img/Gallery/20230919_0.jpg">
    </div>
    <style>
        #slider {
            display: flex;
            justify-content: center;
        }
        #image-container {
            position: relative; 
            width: 100%; 
            height: 600px;
            overflow: hidden; 
        }
        #image-container img {
            position: absolute; 
            top: 0;
            left: 0;
            width: 100%;
            height: 100%; 
            object-fit: contain; 
            opacity: 0; 
            transition: opacity 0.5s ease-in-out;
        }
        #image-container img.active {
            opacity: 1; 
        }
    </style>
    <script>
        var slider = document.getElementById("slider"); 
        var imageContainer = document.getElementById("image-container"); 
        var images = imageContainer.getElementsByTagName("img"); 
        var index = 0; 
        var speed = 3000; 
        function slide() { 
            images[index].classList.remove("active"); 
            index++; 
            if (index >= images.length) {
                index = 0; 
            }
            images[index].classList.add("active"); 
            setTimeout(slide, speed);
        }
        slide();  
    </script>
</div>



