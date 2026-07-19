---
layout: page
title: People
share-description: "Members of the IMPACT Lab at ShanghaiTech University — PhD, master's, and undergraduate researchers in medical imaging AI, led by Dr. Zhiming Cui."
---

<style>
    .rounded-image {
        width: 176px;
        height: 176px;
        border-radius: 50%;
        border: 5px solid #f0f0f0;
        object-fit: cover;
        object-position: center;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        display: block;
        margin: 0 auto 4px;
    }

    .people-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(215px, 1fr));
        gap: 20px;
        margin: 20px 0 40px;
    }

    .person-card {
        display: block;
        text-align: center;
        padding: 22px 15px;
        background-color: #ffffff;
        border-radius: 15px;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .person-card:hover {
        transform: translateY(-6px);
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
    }

    h2 {
        font-size: 2.4em;
        color: #2c3e50;
        margin: 50px 0 35px;
        border-bottom: 3px solid #2c3e50;
        padding-bottom: 12px;
        text-align: center;
    }

    a {
        color: #1a6bd4;
        text-decoration: none;
        font-weight: bold;
        transition: color 0.3s ease;
    }

    a:hover {
        color: #2c3e50;
    }

    .name {
        font-size: 1.3em;
        font-weight: 600;
        margin: 15px 0 8px;
        color: #2c3e50;
    }

    .info {
        font-size: 0.95em;
        color: #7f8c8d;
        line-height: 1.4;
    }

    @media (max-width: 600px) {
        .rounded-image {
            width: 120px;
            height: 120px;
            border-width: 3px;
        }
        h2 {
            font-size: 1.7em;
        }
    }
</style>

{% assign categories = "phd_students,graduate_students,visiting_students,undergraduate_students" | split: "," %}
{% assign titles = "Ph.D. Students,Master's Students,Visiting Students,Undergraduate Students" | split: "," %}

{% for category in categories %}
{% assign people = site.data.people[category] %}
{% if people and people.size > 0 %}
<h2>{{ titles[forloop.index0] }}</h2>
{% include people_table.html people=people id=category %}
{% endif %}
{% endfor %}

{% assign alumni = site.data.people.alumni %}
{% assign alumni_categories = "graduate_students,undergraduate_students,visiting_students" | split: "," %}
{% assign alumni_titles = "Master's Students,Undergraduate Students,Visiting Students" | split: "," %}
{% assign has_alumni = false %}
{% for subcategory in alumni_categories %}
{% assign alumni_people = alumni[subcategory] %}
{% if alumni_people and alumni_people.size > 0 %}
{% assign has_alumni = true %}
{% endif %}
{% endfor %}
{% if has_alumni %}
<h2>Alumni</h2>
{% for subcategory in alumni_categories %}
{% assign alumni_people = alumni[subcategory] %}
{% if alumni_people and alumni_people.size > 0 %}
<h3>{{ alumni_titles[forloop.index0] }}</h3>
{% assign alumni_table_id = "alumni_" | append: subcategory %}
{% include people_table.html people=alumni_people id=alumni_table_id %}
{% endif %}
{% endfor %}
{% endif %}

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
        <img src="/assets/img/Gallery/20240328.jpg" alt="Gallery Image 1" loading="lazy">
        <img src="/assets/img/Gallery/20230919_0.jpg" alt="Gallery Image 2" loading="lazy">
        <img src="/assets/img/Gallery/20230617_2.jpg" alt="Gallery Image 3" loading="lazy">
        <img src="/assets/img/Gallery/UMI2024.png" alt="Gallery Image 4" loading="lazy">
        <img src="/assets/img/Gallery/MLMI2024.jpg" alt="Gallery Image 5" loading="lazy">
        <img src="/assets/img/Gallery/whs.png" alt="Gallery Image 6" loading="lazy">
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
