---
permalink: /
title: "Y-Lab: Intelligent Biomedical Image Processing"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>图片轮播</title>
<style>
  .carousel {
    position: relative;
    width: 600px;
    height: 400px;
    margin: auto;
    overflow: hidden;
  }
  .carousel img {
    width: 100%;
    display: none;
    position: absolute;
    top: 0;
    left: 0;
  }
  .carousel img.active {
    display: block;
  }
  .carousel-indicators {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
  }
  .carousel-indicators span {
    display: inline-block;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background-color: #ccc;
    margin: 0 5px;
    cursor: pointer;
  }
  .carousel-indicators span.active {
    background-color: #333;
  }
  .carousel-btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: #fff;
    border: none;
    cursor: pointer;
    padding: 10px;
  }
  .carousel-btn.prev {
    left: 10px;
  }
  .carousel-btn.next {
    right: 10px;
  }
</style>
</head>
<body>
<br>
<div class="carousel">
  <img src="/images/jiti.png" alt="Image 1" class="active">
  <img src="/images/hainan_tansongbai_1.png" alt="Image 2">
  <img src="/images/hainan_tansongbai_2.png" alt="Image 3">
  <img src="/images/2021graduate.png" alt="Image 4">
  <!-- 更多图片 -->
  <div class="carousel-indicators">
    <span class="active" onclick="moveToSlide(0)"></span>
    <span onclick="moveToSlide(1)"></span>
    <span onclick="moveToSlide(2)"></span>
    <span onclick="moveToSlide(3)"></span>
    <!-- 更多圆点 -->
  </div>
  <button class="carousel-btn prev" onclick="changeSlide(-1)">&#10094;</button>
  <button class="carousel-btn next" onclick="changeSlide(1)">&#10095;</button>
</div>

<script>
  let index = 0;
  const images = document.querySelectorAll('.carousel img');
  const indicators = document.querySelectorAll('.carousel-indicators span');
  const totalImages = images.length;

  function changeSlide(step) {
    images[index].classList.remove('active');
    indicators[index].classList.remove('active');
    index = (index + step + totalImages) % totalImages;
    images[index].classList.add('active');
    indicators[index].classList.add('active');
  }

  function moveToSlide(slideIndex) {
    images[index].classList.remove('active');
    indicators[index].classList.remove('active');
    index = slideIndex;
    images[index].classList.add('active');
    indicators[index].classList.add('active');
  }

  setInterval(() => changeSlide(1), 2000);

  window.onload = () => {
    images[0].classList.add('active');
    indicators[0].classList.add('active');
  };
</script>

</body>
</html>

## 😊About Our Lab
<div style="text-align:justify;">
Welcome to the Guanghui Yue Laboratory, where we focus on <em>1)<strong>Image Quality Assessment and Enhancement</strong></em>, <em>2)<strong>Medical Image Classification</strong></em>, and <em>3)<strong>Medical Image Segmentation</strong></em>. Led by Professor Yue, our team is committed to driving innovation in biomedical imaging. We invite students and researchers to join us in this exciting field and contribute to the advancement of healthcare.
<br> 
<br>
Dr. Guanghui Yue, Ph.D. in Engineering (Tianjin University, supervised by Prof. Chunping Hou), Visiting Scholar at Nanyang Technological University, Singapore (supervised by Prof. Weisi Lin, IEEE/IET Fellow). He is a Tenured Associate Professor, Master's and Ph.D. Supervisor, Shenzhen University. He is a member of the IEEE, and has been leading more than 10 scientific research projects, including the National Natural Science Foundation of China, the Guangdong Province Basic and Applied Basic Research Foundation, etc. His main research directions include sterescopic content processing, image/video quality assessment and enhancement, medical image analysis, machine learning and its applications, etc. To date, he has published more than 70 papers in top-tiered journals and conferences. He serves as a member of the Digital Healthcare and Medical Informatics Branch of the Chinese Society of Biomedical Engineering, an academic committee member of the Artificial Intelligence Branch of Guangdong Medical Association, and a member of the Youth Working Committee of the Chinese Automation Society. He has been a reviewer for more than 20 internationally renowned journals such as IEEE TIP/TMI/TMM/TCSVT/TNNLS/TII/TCYB/TIE/TIM/JBHI/TNSRE/SPL, IET IP/EL, Elsevier SP/DSP/NEUCOM/JVCI/SPIC, etc. 
</div>

## 🔥News
<div style="text-align:justify;">
<ol>
  <li>2024-08-31: One Paper entitled <a href="https://ieeexplore.ieee.org/Xplore/home.jsp">"Unsupervised Low-Light Image Enhancement with Self-Paced Learning"</a> is accepted by <em>IEEE Transactions on Multimedia</em>. &#x1F44F;&#x1F44F;&#x1F44F;</li>
  <li>2024-07-16: One Paper entitled <a href="https://ieeexplore.ieee.org/Xplore/home.jsp">"Progressive Region-to-Boundary Exploration Network for Camouflaged Object Detection"</a> is accepted by <em>IEEE Transactions on Multimedia</em>. &#x1F44F;&#x1F44F;&#x1F44F;</li>
</ol>
</div>

## 🤝Parters
- [Tianwei Zhou](https://cm.szu.edu.cn/Faculty/Management_Science/ZHOU_Tianwei.htm)
- [Wei Zhou](https://weizhou-geek.github.io)


## 🙋For more info
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
