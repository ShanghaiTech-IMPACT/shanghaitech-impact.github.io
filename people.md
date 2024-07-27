---
layout: page
title: People
---

<style>
    .rounded-image {
        width: 200px;
        height: 200px;
        border-radius: 50%;
        border: 5px solid rgb(192, 192, 192);
        object-fit: cover; 
        object-position: center;
    }

    
    @media (max-width: 600px) {
        .rounded-image {
            width: 100px;  
            height: 100px;  
            border-radius: 50%;
            border: 3px solid rgb(192, 192, 192);  
            object-fit: cover;
            object-position: center;
        }
    }

    table {
        width: 100%;
        table-layout: fixed;
        border-collapse: collapse; 
    }

    td {
        width: 25%;
        text-align: center;
        vertical-align: top;
        border: none;
    }
</style>


## Ph.D. Students

<html>
    <table class="people" id="students">
        <tr>
            <td>
                <img src="/assets/img/people/HanWu.png" class="rounded-image"><br>
                <a href="http://hanwu.website/">Han Wu</a><br>
                Ph.D. since 2022<br>
                B.E. WUT
            </td>
            <td>
                <img src="/assets/img/people/ZhentaoLiu.jpg" class="rounded-image"><br>
                <a href="https://github.com/Zhentao-Liu/">Zhentao Liu</a><br>
                Ph.D. since 2022<br>
                B.E. NBU
            </td>
            <td>
                &nbsp;
            </td>
            <td>
                &nbsp;
            </td>
        </tr>
    </table>
</html>

## Graduate Students

<table class="people" id="students">
    <tr>
        <td>
            <img src="/assets/img/people/HaoshenWang.jpg" class="rounded-image"><br>
            Haoshen Wang<br>
            M.S. since 2022<br>
            B.E. DUT
        </td>
        <td>
            <img src="/assets/img/people/YulongDou.jpg" class="rounded-image"><br>
            <a href="https://douyl.github.io/">Yulong Dou</a><br>  
            M.S. since 2023<br>
            B.E. ShanghaiTech
        </td>
        <td>
            <img src="/assets/img/people/ChenfanXu.png" class="rounded-image"><br>
            Chenfan Xu<br>
            M.S. since 2023<br>
            B.E. SHU
        </td>
        <td>
            <img src="/assets/img/people/XingyueWang.jpg" class="rounded-image"><br>
            Xingyue Wang<br>
            M.S. since 2023<br>
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
                M.S. from NEU
            </td>
            <td>
                <img src="/assets/img/people/ZichenZhang.jpg" class="rounded-image"><br>
                Zichen Zhang<br>
                M.S. from TUM
            </td>
            <td>
                &nbsp;
            </td>
        </tr>
    </table>
</html>


## Undergraduate Students
<html>
    <table class="people" id="students">
        <tr>
        <td>
                <img src="/assets/img/people/SiyuChen.jpeg" class="rounded-image"><br>
                Siyu Chen<br>
                Class 2021<br>
            </td>
            <td>
                 <img src="/assets/img/people/WeiJia.png" class="rounded-image"><br>
                Wei Jia<br>
                Class 2022<br>
            </td>
            <td>
                <img src="/assets/img/people/JinzeWu.jpg" class="rounded-image"><br>
                Jinze Wu<br>
                Class 2022<br>
            </td>
            <td>
                &nbsp;
            </td>
        </tr>
    </table>
</html>


<!-- <h3>Gallery </h3> -->
## Gallery
<style>
    #slider {
        display: flex;
        justify-content: center;
    }
    #image-container {
        position: relative; 
        width: 100%;  
        padding-top: 56.25%; /* 16:9 Aspect Ratio */
        height: 0; /* Height is now controlled by padding */
        overflow: hidden; 
    }
    #image-container img {
        position: absolute; 
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        max-width: 100%;
        max-height: 100%;
        object-fit: contain; 
        opacity: 0; 
        transition: opacity 0.5s ease-in-out;
    }
    #image-container img.active {
        opacity: 1; 
    }
</style>


<div id="slider">
    <div id="image-container">
        <img src="/assets/img/Gallery/20240328.jpg">
        <img src="/assets/img/Gallery/20230919_0.jpg">
        <img src="/assets/img/Gallery/20230617_2.jpg">
    </div>
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



