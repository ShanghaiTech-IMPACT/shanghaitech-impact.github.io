---
layout: page
title: Milestones
---

<div class="timeline">
    <div class="timeline-item">
        <div class="timeline-date">September 2022</div>
        <div class="timeline-content">
            <h3>IMPACT Lab Established</h3>
            <p>IMPACT Lab is officially founded at ShanghaiTech University, marking the beginning of our journey in medical imaging research.</p>
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-date">September 2022</div>
        <div class="timeline-content">
            <h3>First Members of IMPACT Lab</h3>
            <p>Han Wu, Zhentao Liu and Haoshen Wang join as the first members of IMPACT Lab, setting the foundation for our research team.</p>
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-date">June 2023</div>
        <div class="timeline-content">
            <h3>First MICCAI Paper</h3>
            <p>Han Wu authors our lab's first paper accepted at MICCAI conference, showcasing our early research achievements.</p>
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-date">October 2023</div>
        <div class="timeline-content">
            <h3>First National Scholarship Award (Master)</h3>
            <p>Yulong Dou becomes the first member of IMPACT Lab to receive the National Scholarship at the Master's level.</p>
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-date">June 2024</div>
        <div class="timeline-content">
            <h3>Dr. Cui reaches 1k Citations</h3>
            <p>Dr. Cui, the founder of IMPACT Lab, reaches a milestone of 1,000 citations for his research work, highlighting the lab's growing influence in the field of medical imaging.</p>
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-date">July 2024</div>
        <div class="timeline-content">
            <h3>PhD and new EngD Students</h3>
            <p>We celebrate Han Wu and Zhentao Liu's success in passing their PhD Qualifying Exams (PQE), officially becoming PhD candidates. Additionally, we warmly welcome Ruochen Pi, our new EngD student, to the IMPACT Lab family.</p>
        </div>
    </div>
    <div class="timeline-item">
        <div class="timeline-date">October 2024</div>
        <div class="timeline-content">
            <h3>First TMI Publication</h3>
            <p>Zhentao Liu leads the publication of our lab's first paper in the IEEE Transactions on Medical Imaging (TMI) journal.</p>
        </div>
    </div>
</div>

<style>
    .timeline {
        position: relative;
        max-width: 1200px;
        margin: 0 auto;
        padding: 40px 0;
        font-family: 'Arial', sans-serif;
    }
    .timeline::after {
        content: '';
        position: absolute;
        width: 4px;
        background-color: #3498db;
        top: 0;
        bottom: 0;
        left: 50%;
        margin-left: -2px;
        box-shadow: 0 0 10px rgba(52, 152, 219, 0.5);
    }
    .timeline-item {
        padding: 20px 40px;
        position: relative;
        background-color: inherit;
        width: 50%;
        box-sizing: border-box;
    }
    .timeline-item::after {
        content: '';
        position: absolute;
        width: 20px;
        height: 20px;
        right: -10px;
        background-color: #fff;
        border: 4px solid #3498db;
        top: 20px;
        border-radius: 50%;
        z-index: 1;
        transition: all 0.3s ease;
        box-shadow: 0 0 0 4px rgba(52, 152, 219, 0.2);
    }
    .timeline-item:hover::after {
        background-color: #3498db;
        transform: scale(1.2);
    }
    .timeline-item:nth-child(odd) {
        left: 0;
    }
    .timeline-item:nth-child(even) {
        left: 50%;
    }
    .timeline-item:nth-child(even)::after {
        left: -10px;
    }
    .timeline-content {
        padding: 20px;
        background-color: white;
        position: relative;
        border-radius: 10px;
        box-shadow: 0 8px 16px rgba(0,0,0,0.1);
        transition: all 0.3s ease;
    }
    .timeline-content:hover {
        transform: translateY(-5px);
        box-shadow: 0 12px 24px rgba(0,0,0,0.15);
    }
    .timeline-date {
        font-weight: bold;
        color: #3498db;
        margin-bottom: 10px;
        font-size: 1.2em;
        text-transform: uppercase;
        letter-spacing: 1px;
    }
    .timeline-content h3 {
        margin-top: 0;
        color: #2c3e50;
        font-size: 1.6em;
        margin-bottom: 10px;
    }
    .timeline-content p {
        margin-bottom: 0;
        line-height: 1.8;
        color: #34495e;
        font-size: 1.1em;
    }
    @media screen and (max-width: 768px) {
        .timeline::after {
            left: 30px;
        }
        .timeline-item {
            width: 100%;
            padding-left: 70px;
            padding-right: 25px;
        }
        .timeline-item::after {
            left: 20px;
        }
        .timeline-item:nth-child(even) {
            left: 0%;
        }
    }
</style>