---
layout: page
title: Research
share-description: "Research at the IMPACT Lab, ShanghaiTech University: medical image computing, image reconstruction (CBCT/DSA/PET-CT), and digital dentistry, with representative publications."
---

<style>
    .research-section {
        margin-bottom: 40px;
        padding: 30px;
        background-color: #ffffff;
        border-radius: 15px;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        scroll-margin-top: 80px;
    }
    .research-section h2 {
        font-size: 1.9em;
        color: #2c3e50;
        margin: 0 0 20px;
        border-bottom: 3px solid #2c3e50;
        padding-bottom: 12px;
    }
    .research-section > p {
        font-size: 1.08em;
        line-height: 1.75;
        color: #34495e;
    }
    .research-section a {
        color: #1a6bd4;
        text-decoration: none;
    }
    .research-section a:hover {
        color: #0f3d73;
        text-decoration: underline;
    }
    .rep-grid {
        display: grid;
        grid-template-columns: repeat(3, minmax(0, 1fr));
        gap: 16px;
        margin: 18px 0 6px;
    }
    .rep-card {
        border: 1px solid #e5e9ee;
        border-radius: 10px;
        background: #ffffff;
        overflow: hidden;
        display: flex;
        flex-direction: column;
        transition: box-shadow 0.25s ease, transform 0.25s ease;
    }
    .rep-card:hover {
        transform: translateY(-3px);
        box-shadow: 0 6px 14px rgba(0, 0, 0, 0.12);
    }
    .rep-card img {
        width: 100%;
        height: 140px;
        object-fit: contain;
        background: #f8f9fa;
        padding: 8px;
    }
    .rep-info {
        padding: 12px 14px 14px;
        display: flex;
        flex-direction: column;
        gap: 6px;
        flex: 1;
    }
    .rep-title {
        font-size: 0.93em;
        font-weight: 600;
        line-height: 1.4;
        color: #24292e;
    }
    .rep-title a {
        color: inherit;
    }
    .rep-venue {
        font-size: 0.85em;
        color: #586069;
        margin-top: auto;
    }
    .rep-links {
        font-size: 0.85em;
    }
    .rep-more {
        font-size: 0.98em;
        color: #586069;
        margin: 14px 0 0;
    }
    @media (max-width: 768px) {
        .research-section {
            padding: 22px 18px;
        }
        .rep-grid {
            grid-template-columns: 1fr;
        }
        .rep-card img {
            height: 160px;
        }
    }
</style>

<div class="research-section" id="medical-image-computing">
    <h2>Medical Image Computing</h2>
    <p>We develop learning-based methods for segmentation, landmark detection, and localization across CT, CBCT, MRI, and X-ray images, with a particular focus on robustness when annotations are scarce — including semi-supervised, cross-domain, and prototype-based learning. Beyond methodology, we validate our systems in multi-center clinical studies with close clinical collaborators.</p>
    <div class="rep-grid">
        <div class="rep-card">
            <img src="/assets/img/publications/2026_ThinTubularSeg.png" alt="Anatomical prior-guided implicit segmentation of thin and tubular structures" loading="lazy">
            <div class="rep-info">
                <div class="rep-title">Anatomical Prior-guided Implicit Segmentation of Challenging Thin and Tubular Anatomical Structures in CBCT Images</div>
                <div class="rep-venue">MedIA, 2026</div>
            </div>
        </div>
        <div class="rep-card">
            <img src="/assets/img/publications/2025_DuCiSC.png" alt="DuCiSC semi-supervised segmentation framework" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://ieeexplore.ieee.org/abstract/document/11104231">Dual Cross-image Semantic Consistency with Self-aware Pseudo Labeling for Semi-supervised Medical Image Segmentation</a></div>
                <div class="rep-venue">IEEE TMI, 2025</div>
                <div class="rep-links">[<a href="https://ieeexplore.ieee.org/abstract/document/11104231">paper</a>] [<a href="https://github.com/ShanghaiTech-IMPACT/DuCiSC/">code</a>]</div>
            </div>
        </div>
        <div class="rep-card">
            <img src="/assets/img/publications/2026_SemiEchoTracker.png" alt="Semi-supervised landmark tracking in echocardiography video" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://doi.org/10.1109/TMI.2026.3651389">Semi-Supervised Landmark Tracking in Echocardiography Video via Spatial-Temporal Co-Training and Perception-Aware Attention</a></div>
                <div class="rep-venue">IEEE TMI, 2026</div>
                <div class="rep-links">[<a href="https://doi.org/10.1109/TMI.2026.3651389">paper</a>] [<a href="https://github.com/Fitz-Fitz/SemiEchoTracker">code</a>]</div>
            </div>
        </div>
    </div>
    <p class="rep-more">More in <a href="/publications/">Publications</a>.</p>
</div>

<div class="research-section" id="image-reconstruction">
    <h2>Image Reconstruction</h2>
    <p>We study learning-based reconstruction for CBCT, DSA, and PET/CT — recovering high-quality 3D and 4D structures from sparse-view, low-dose, or artifact-corrupted acquisitions. Our recent work builds on implicit neural representations, radiative Gaussian splatting for dynamic vessel reconstruction, and 3D diffusion models for controllable, high-fidelity medical image generation.</p>
    <div class="rep-grid">
        <div class="rep-card">
            <img src="/assets/img/publications/2026_VPAL.png" alt="Vessel probability guided attenuation learning for DSA reconstruction" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://www.sciencedirect.com/science/article/pii/S136184152600157X?via=ihub">3D Vessel Reconstruction from Sparse-View Dynamic DSA Images via Vessel Probability Guided Attenuation Learning</a></div>
                <div class="rep-venue">MedIA, 2026</div>
                <div class="rep-links">[<a href="https://www.sciencedirect.com/science/article/pii/S136184152600157X?via=ihub">paper</a>] [<a href="https://github.com/ShanghaiTech-IMPACT/VPAL">code</a>]</div>
            </div>
        </div>
        <div class="rep-card">
            <img src="/assets/img/publications/2024_cbct_reconstruction.png" alt="Geometry-aware attenuation learning for sparse-view CBCT reconstruction" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://ieeexplore.ieee.org/abstract/document/10705334">Geometry-Aware Attenuation Learning for Sparse-View CBCT Reconstruction</a></div>
                <div class="rep-venue">IEEE TMI, 2024</div>
                <div class="rep-links">[<a href="https://ieeexplore.ieee.org/abstract/document/10705334">paper</a>] [<a href="https://github.com/ShanghaiTech-IMPACT/Geometry-Aware-Attenuation-Learning-for-Sparse-View-CBCT-Reconstruction">code</a>]</div>
            </div>
        </div>
        <div class="rep-card">
            <img src="/assets/img/publications/2024_3DMedDiffusion.png" alt="3D MedDiffusion medical image generation" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://arxiv.org/abs/2412.13059">3D MedDiffusion: A 3D Medical Diffusion Model for Controllable and High-quality Medical Image Generation</a></div>
                <div class="rep-venue">IEEE TMI, 2025</div>
                <div class="rep-links">[<a href="https://arxiv.org/abs/2412.13059">paper</a>] [<a href="https://github.com/ShanghaiTech-IMPACT/3D-MedDiffusion/">code</a>]</div>
            </div>
        </div>
    </div>
    <p class="rep-more">More in <a href="/publications/">Publications</a>.</p>
</div>

<div class="research-section" id="digital-dentistry">
    <h2>Digital Dentistry</h2>
    <p>We build full-stack AI for digital dentistry: tooth and alveolar bone segmentation from CBCT, clinical knowledge-informed tooth alignment for orthodontic planning, 3D teeth reconstruction from intra-oral photographs, and automated diagnosis of periodontal disease and dental caries. This line of work is carried out with close clinical collaborators and has produced several open benchmarks — CBCT segmentation, cephalometric landmarks (CephAdoAdu), tooth alignment, and caries detection (DVCT) — released on our <a href="/dataset/">Dataset</a> page.</p>
    <div class="rep-grid">
        <div class="rep-card">
            <img src="/assets/img/publications/2022_NC.png" alt="Fully automatic tooth and alveolar bone segmentation system" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://www.nature.com/articles/s41467-022-29637-2.pdf">A Fully Automatic AI System for Tooth and Alveolar Bone Segmentation from Cone-beam CT Images</a></div>
                <div class="rep-venue">Nature Communications, 2022</div>
                <div class="rep-links">[<a href="https://www.nature.com/articles/s41467-022-29637-2.pdf">paper</a>] [<a href="https://github.com/ErdanC/Tooth-and-alveolar-bone-segmentation-from-CBCT">code</a>]</div>
            </div>
        </div>
        <div class="rep-card">
            <img src="/assets/img/publications/2025_tooth_alignment.png" alt="CLIK-Diffusion tooth alignment" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://www.sciencedirect.com/science/article/pii/S1361841525002932?dgcid=author">CLIK-Diffusion: Clinical Knowledge-informed Diffusion Model for Tooth Alignment</a></div>
                <div class="rep-venue">MedIA, 2025</div>
                <div class="rep-links">[<a href="https://www.sciencedirect.com/science/article/pii/S1361841525002932?dgcid=author">paper</a>] [<a href="https://github.com/ShanghaiTech-IMPACT/CLIK-Diffusion">code</a>]</div>
            </div>
        </div>
        <div class="rep-card">
            <img src="/assets/img/publications/2025_CRM.png" alt="PerioAI digital periodontal diagnosis system" loading="lazy">
            <div class="rep-info">
                <div class="rep-title"><a href="https://www.sciencedirect.com/science/article/pii/S2666379125002599">PerioAI: A Digital System for Periodontal Disease Diagnosis from an Intra-oral Scan and Cone-beam CT Image</a></div>
                <div class="rep-venue">Cell Reports Medicine, 2025</div>
                <div class="rep-links">[<a href="https://www.sciencedirect.com/science/article/pii/S2666379125002599">paper</a>]</div>
            </div>
        </div>
    </div>
    <p class="rep-more">More in <a href="/publications/">Publications</a> · Open benchmarks in <a href="/dataset/">Dataset</a>.</p>
</div>
