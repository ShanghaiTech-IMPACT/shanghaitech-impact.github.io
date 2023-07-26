---
layout: page
title: People
---



## Graduate Students
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


<table class="people" id="students">
    <tr>
        <td>
            <img src="/assets/img/people/HanWu.jpg" class="rounded-image"><br>
            <a href="http://hanwu.website/">Han Wu</a><br>
            M.S. since 2022<br>
            B.E. WUT
        </td>
        <td>
            <img src="/assets/img/people/ZhentaoLiu.png" class="rounded-image"><br>
            Zhentao Liu<br>
            M.S. since 2022<br>
            B.E. NBU
        </td>
        <td>
            <img src="/assets/img/people/HaoshenWang.jpg" class="rounded-image"><br>
            Haoshen Wang<br>
            M.S. since 2022<br>
            B.E. DUT
        </td>
    </tr>
    <tr>
        <td>
            <img src="/assets/img/people/YulongDou.jpg" class="rounded-image"><br>
            Yulong Dou<br>
            M.S. since 2023<br>
            B.E. ShanghaiTech
        </td>
        <td>
            <img src="/assets/img/people/ChenfanXu.jpg" class="rounded-image"><br>
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
</table>






## Visiting Students
<html>
    <table class="people" id="students">
        <tr>
            <td>
                <img src="/assets/img/people/QingyaoLuo.jpg" class="rounded-image"><br>
                Qingyao Luo<br>
                M.S. from Northeastern University
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

<!-- <h3>Gallery </h3> -->
## Gallery
<div id="slider">
    <div id="image-container">
        <img src="/assets/img/Gallery/20230617_0.jpg">
        <img src="/assets/img/Gallery/20230617_1.jpg">
        <img src="/assets/img/Gallery/20230617_2.jpg">
    </div>
    <style>
        #slider {
            display: flex;
            justify-content: center;
        }
        #image-container {
            position: relative; /* 设置容器为相对定位 */
            width: 100%; /* 设置容器宽度 */
            height: 600px; /* 设置容器高度 */
            overflow: hidden; /* 隐藏超出容器的部分 */
        }
        #image-container img {
            position: absolute; /* 设置图片为绝对定位 */
            top: 0;
            left: 0;
            width: 100%; /* 设置图片宽度为容器宽度 */
            height: 100%; /* 设置图片高度为容器高度 */
            object-fit: contain; 
            opacity: 0; /* 初始设置图片透明度为0 */
            transition: opacity 0.5s ease-in-out; /* 添加过渡效果 */
        }
        #image-container img.active {
            opacity: 1; /* 设置当前图片透明度为1 */
        }
    </style>
    <script>
        var slider = document.getElementById("slider"); // 获取滚动播放图片的父元素
        var imageContainer = document.getElementById("image-container"); // 获取图片容器
        var images = imageContainer.getElementsByTagName("img"); // 获取所有滚动播放图片的集合
        var index = 0;  // 设置初始索引和滚动速度
        var speed = 3000; // 每张图片滚动的间隔时间（以毫秒为单位）
        function slide() { // 定义滚动函数
            images[index].classList.remove("active"); // 移除当前图片的active类
            index++; // 增加索引
            if (index >= images.length) {
                index = 0; // 如果索引超出范围，则重置为0
            }
            images[index].classList.add("active"); // 添加下一张图片的active类
            setTimeout(slide, speed); // 设置下一次滚动的定时器
        }
        slide();  // 调用滚动函数开始滚动播放图片
    </script>
</div>



