---
layout: page
---
<style>
body {
  background-color: #f0f5fa;  /* A very light blue background */
  position: relative;
  overflow-x: hidden; /* Prevent horizontal scrollbar */
}

/* Page flowing light effect */
body::before {
  content: '';
  position: fixed;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(100, 180, 255, 0.2), transparent);
  z-index: -1;
  animation: page-flow-light 8s infinite linear;
  pointer-events: none;
}

/* Flowing light animation */
@keyframes page-flow-light {
  0% { left: -100%; }
  100% { left: 100%; }
}

.scrollable-news {
  max-height: 400px;
  overflow-y: auto;
  border-radius: 12px;
  padding: 15px;
  background-color: #f8fbff;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  margin: 15px 0;
  list-style: none;
}

.scrollable-news li {
  margin-bottom: 4px;
  padding: 5px;
  border-bottom: 1px solid #e6f0ff;
  line-height: 1.4;
}

.scrollable-news li:hover {
  background-color: #e6f2ff;
  transition: background-color 0.3s ease;
}

.scrollable-news li:last-child {
  border-bottom: none;
}

.scrollable-news::-webkit-scrollbar {
  width: 8px;
}

.scrollable-news::-webkit-scrollbar-track {
  background: #f1f1f1;
  border-radius: 10px;
}

.scrollable-news::-webkit-scrollbar-thumb {
  background: #c0c0c0;
  border-radius: 10px;
}

.scrollable-news::-webkit-scrollbar-thumb:hover {
  background: #a0a0a0;
}

.mouse-particle {
  pointer-events: none;
  position: fixed;
  border-radius: 50%;
  background: rgba(255, 215, 0, 0.25);
  box-shadow: 0 0 10px rgba(207, 187, 74, 0.3);
  z-index: 10000;
  transform: translate(-50%, -50%);
}

.profile-image {
  aspect-ratio: 1.624;  /* 4724/2910 ≈ 1.624 */
  object-fit: cover;
}

@media screen and (max-width: 768px) {
  .profile-image {
    width: 100% !important;
    max-width: 400px !important;
    float: none !important;
    margin: 1em auto !important;
    display: block;
  }
}
</style>

# About Me

<img src="images/JianyuLai_img5_20250702.jpg" class="floatpic profile-image" style="width: 43%; max-width: 400px; height: auto; float: right; margin-left: 1.5em; margin-bottom: 1em; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

<!-- My name is **Jianyu Lai (赖建宇)**. I am a Master of Philosophy student in Data Science and Analytics at The Hong Kong University of Science and Technology (Guangzhou), supervised by Prof. Lei Zhu. I earned my Bachelor's degree in Automation Engineering from South China University of Technology. During my undergraduate studies, I was a vision team member for the RoboMaster University Championship 2022, where our team won the National First Prize. Concurrently, I independently developed an automatic focusing system based on depth vision. Currently, as an MPhil student, I am involved in a Red Bird project focused on the Research and Development of More Capable and Intelligent UAV and Novel Applications.

My graduate studies have further fueled my strong interest in low-level vision and AIGC. I am fortunate that my first paper has been accepted by CVPR 2025, and I am actively exploring new frontiers in these areas, including computational photography.

If you are interested in my work or research, please feel free to contact me. -->

<!-- My name is **Jianyu Lai (赖建宇)**. I am a Master of Philosophy student in Data Science and Analytics at The Hong Kong University of Science and Technology (Guangzhou), supervised by Prof. Lei Zhu. My graduate studies have further fueled my strong interest in low-level vision and AIGC. I am fortunate that my first paper has been accepted by CVPR 2025, and I am actively exploring new frontiers in these areas, including computational photography.

If you are interested in my work or research, please feel free to contact me. -->

My name is **Jianyu Lai (赖建宇)**. I am a Master of Philosophy student in Data Science and Analytics at The Hong Kong University of Science and Technology (Guangzhou), supervised by Prof. Lei Zhu. During my graduate studies, I have developed a strong interest and focus on **low-level vision**, **computational photography**, and **AIGC** (Artificial Intelligence Generated Content). I am fortunate that my first paper has been accepted by CVPR 2025, and I am actively exploring new frontiers in these areas. Notably, my recent work includes **Postercraft**, an end-to-end poster generation project that leverages cutting-edge AIGC techniques.

If you are interested in my work or research, please feel free to contact me.


<br>

## Education

- **Sept. 2024 – Present:** The Hong Kong University of Science and Technology (Guangzhou)  
  *Master of Philosophy in Data Science and Analytics (DSA)*
- **Sept. 2020 – June 2024:** South China University of Technology  
  *Bachelor of Engineering in Automation*

<br>

---

## Research Interests

- Researching Advanced AIGC algorithms and their applications, such as photography generation, poster generation, text generation, and image editing.
- Developing robust and generalizable solutions for degraded image restoration, particularly in complex real-world scenarios.
- Exploring multimodal large language models (MLLM) for image processing and evaluation.

<br>

---

## News and Updates

<div class="scrollable-news">
 <ul>
  <li><strong>Jun. 2025:</strong> Our work <em><a href="https://ephemeral182.github.io/GenHaze/" target="_blank">GenHaze: Pioneering Controllable One-Step Realistic Haze Generation for Real-World Dehazing</a></em> has been accepted by ICCV 2025!</li>
  <li><strong>Jun. 2025:</strong> We released our latest work, <em><a href="https://arxiv.org/abs/2506.10741" target="_blank">PosterCraft: Rethinking High-Quality Aesthetic Poster Generation in a Unified Framework</a></em>, on Arxiv.</li>
  <li><strong>Mar. 2025:</strong> Luckily, our paper <em><a href="https://openaccess.thecvf.com/content/CVPR2025/papers/Lai_SnowMaster_Comprehensive_Real-world_Image_Desnowing_via_MLLM_with_Multi-Model_Feedback_CVPR_2025_paper.pdf" target="_blank">SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization</a></em> was accepted by CVPR 2025.</li>
  <li><strong>Sept. 2024:</strong> Began my MPhil program in Data Science and Analytics at HKUST (Guangzhou).</li>
  <li><strong>Aug. 2022:</strong> Awarded the National First Prize at the RoboMaster University Championship as a technical team member.</li>
  <li><strong>Jun. 2023:</strong> Granted a patent for an automatic focusing system based on depth vision and target detection.</li>
 </ul>
</div>

<!-- <br>

---

## Projects

- **Gait Face Fusion Recognition System Based on Multi Perspective Collaboration:**  
  A national-level project developing a multi-person gait recognition system with a visual interface that integrates facial and gait features. I led the design and implementation of the occlusion gait restoration module to significantly improve recognition accuracy.

- **Auto-Focus-Assistant:**  
  An independent R&D project leveraging depth cameras and advanced computer vision techniques to deliver an efficient auto-focus system. It processes both spatial depth and RGB data via YolofastestV2 for object detection, supporting multiple focusing modes (manual, automatic, continuous tracking).

- **Original Aspiration: RoboMaster Short Film Project:**  
  A team-driven filmmaking project where I served as the team leader, overseeing screenwriting, directing, cinematography, and post-production. The short film documents the journey of preparing for a robotics competition and has received positive attention.

- **National College Student Robot Competition (RoboMaster University Championship):**  
  A robotics contest in which I participated as a UAV team member; responsible for designing and developing the target detection system, assisting in debugging and flight testing, as well as maintaining the robot vision repository.

<br> -->

---

## Awards

- **Patent (Jun. 2023):** Inventor of an automatic focusing system based on depth vision and target detection (Patent CN219268990U).
- **National First Prize (Aug. 2022):** Awarded as a technical team member in the RoboMaster University Championship.

<br>

<script>
// Mouse particle effect
document.addEventListener('DOMContentLoaded', function() {
  function createParticle(x, y, size) {
    const particle = document.createElement('div');
    particle.className = 'mouse-particle';
    const actualSize = size * (0.5 + Math.random() * 0.5);
    particle.style.width = actualSize + 'px';
    particle.style.height = actualSize + 'px';
    const hue = Math.floor(Math.random() * 360);
    particle.style.background = `hsla(${hue}, 80%, 60%, 0.25)`;
    particle.style.boxShadow = `0 0 10px hsla(${hue}, 80%, 50%, 0.3)`;
    particle.style.left = x + 'px';
    particle.style.top = y + 'px';
    document.body.appendChild(particle);
    setTimeout(() => {
      particle.style.opacity = '0';
      particle.style.transform = 'translate(-50%, -50%) scale(0.5)';
      particle.style.transition = 'all 0.6s ease-out';
      setTimeout(() => {
        document.body.removeChild(particle);
      }, 600);
    }, 10);
  }
  
  let lastX = 0, lastY = 0, throttle = false;
  document.addEventListener('mousemove', function(e) {
    if (throttle) return;
    throttle = true;
    setTimeout(() => { throttle = false; }, 10);
    const x = e.clientX, y = e.clientY;
    const speed = Math.sqrt(Math.pow(x - lastX, 2) + Math.pow(y - lastY, 2));
    const size = Math.min(16, Math.max(5, speed * 0.4));
    createParticle(x, y, size);
    lastX = x; lastY = y;
  });
});
</script>

---