---
layout: page
title: People
---

<style>
    .rounded-image {
        width: 200px;
        height: 200px;
        border-radius: 50%;
        border: 5px solid #f0f0f0;
        object-fit: cover; 
        object-position: center;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
    }

    .rounded-image:hover {
        transform: scale(1.05) translateY(-5px);
        box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
        border-color:rgb(0, 0, 0);
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
        padding: 25px;
        background-color: #ffffff;
        border-radius: 15px;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
        transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
        position: relative;
        overflow: hidden;
    }

    .people td:hover {
        transform: translateY(-8px);
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
    }

    .people td::after {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.1), transparent);
        transform: translateX(-100%);
        transition: 0.5s;
    }

    .people td:hover::after {
        transform: translateX(100%);
    }

    /* Add this new style for empty cells */
    .people td.empty-cell {
        background-color: transparent;
        box-shadow: none;
        padding: 0;
        pointer-events: none;
    }
    
    /* Disable all hover effects for empty cells */
    .people td.empty-cell:hover {
        transform: none;
        box-shadow: none;
    }
    
    .people td.empty-cell::after {
        content: none;
    }

    h2 {
        font-size: 2.4em;
        color: #2c3e50;
        margin: 50px 0 35px;
        border-bottom: 3px solid #2c3e50;
        padding-bottom: 12px;
        text-align: center;
        position: relative;
    }

    h2::after {
        content: '';
        position: absolute;
        bottom: -3px;
        left: 50%;
        transform: translateX(-50%);
        width: 60px;
        height: 3px;
    }

    a {
        color: #4db8ff;
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
        line-height: 1.6;
    }
</style>

{% assign categories = "phd_students,graduate_students,visiting_students,undergraduate_students,alumni" | split: "," %}
{% assign titles = "Ph.D. Students,Graduate Students,Visiting Students,Undergraduate Students,Alumni" | split: "," %}

{% for category in categories %}
<h2>{{ titles[forloop.index0] }}</h2>

<table class="people" id="{{ category }}">
    <tr>
        {% assign people = site.data.people[category] %}
        {% for person in people %}
            <td>
                <img src="{{ person.image }}" class="rounded-image" alt="{{ person.name }}">
                <div class="name">
                    {% if person.url %}
                        <a href="{{ person.url }}">{{ person.name }}</a>
                    {% else %}
                        {{ person.name }}
                    {% endif %}
                </div>
                <div class="info">{{ person.info }}</div>
                {% if person.education %}
                    <div class="info">{{ person.education }}</div>
                {% endif %}
                {% if person.period %}
                    <div class="info">{{ person.period }}</div>
                {% endif %}
                {% if person.note != "" %}
                    <div class="info">{{ person.note }}</div>
                {% endif %}
            </td>
            {% assign remainder = forloop.index | modulo: 4 %}
            {% if remainder == 0 and forloop.index != forloop.length %}
                </tr><tr>
            {% endif %}
        {% endfor %}
        {% assign empty_cells = 4 | minus: remainder %}
        {% if remainder != 0 %}
            {% for i in (1..empty_cells) %}
                <td class="empty-cell"></td>
            {% endfor %}
        {% endif %}
    </tr>
</table>
{% endfor %}

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
        <img src="/assets/img/Gallery/whs.png" alt="Gallery Image 6">
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