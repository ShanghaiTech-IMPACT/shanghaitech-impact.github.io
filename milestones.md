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
            <h3>PhD and EngD Students</h3>
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
    <div class="timeline-item">
        <div class="timeline-date">February 2025</div>
        <div class="timeline-content">
            <h3>First IPMI Paper</h3>
            <p>Zhentao Liu presents our lab's first paper in the Information Processing in Medical Imaging (IPMI) conference.</p>
        </div>
    </div>
</div>

<style>
    .timeline {
        position: relative;
        max-width: 1200px;
        margin: 0 auto;
        padding: 60px 0;
        font-family: 'Roboto', 'Arial', sans-serif;
    }
    .timeline::after {
        content: '';
        position: absolute;
        width: 3px;
        background: linear-gradient(to bottom, #2196F3, #03A9F4);
        top: 0;
        bottom: 0;
        left: 50%;
        margin-left: -1.5px;
        box-shadow: 0 0 15px rgba(33, 150, 243, 0.3);
    }
    .timeline-item {
        padding: 30px 50px;
        position: relative;
        background-color: inherit;
        width: 50%;
        box-sizing: border-box;
        transition: all 0.4s ease;
    }
    .timeline-item::after {
        content: '';
        position: absolute;
        width: 24px;
        height: 24px;
        right: -12px;
        background-color: #fff;
        border: 4px solid #2196F3;
        top: 30px;
        border-radius: 50%;
        z-index: 1;
        transition: all 0.4s ease;
        box-shadow: 0 0 0 4px rgba(33, 150, 243, 0.2);
    }
    .timeline-item:hover::after {
        background-color: #2196F3;
        transform: scale(1.3);
        box-shadow: 0 0 0 6px rgba(33, 150, 243, 0.3);
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
        padding: 25px;
        background: linear-gradient(145deg, #ffffff, #f5f5f5);
        position: relative;
        border-radius: 15px;
        box-shadow: 0 10px 20px rgba(0,0,0,0.08);
        transition: all 0.4s ease;
    }
    .timeline-content:hover {
        transform: translateY(-8px);
        box-shadow: 0 15px 30px rgba(0,0,0,0.12);
    }
    .timeline-date {
        font-weight: 600;
        color: #2196F3;
        margin-bottom: 12px;
        font-size: 1.1em;
        text-transform: uppercase;
        letter-spacing: 1.5px;
        position: relative;
        display: inline-block;
    }
    .timeline-date::after {
        content: '';
        position: absolute;
        bottom: -4px;
        left: 0;
        width: 40%;
        height: 2px;
        background-color: #2196F3;
    }
    .timeline-content h3 {
        margin-top: 0;
        color: #1a1a1a;
        font-size: 1.7em;
        margin-bottom: 15px;
        font-weight: 600;
    }
    .timeline-content p {
        margin-bottom: 0;
        line-height: 1.9;
        color: #424242;
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