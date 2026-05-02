---
title: "Curriculum Vitae / 个人简历"
layout: splash
permalink: /cv/
---

<div class="lang-toggle-container">
  <span class="lang-label" id="label-en" style="color: #007bff;">English</span>
  <label class="switch">
    <input type="checkbox" id="langSwitch" onchange="toggleLanguage()">
    <span class="slider round"></span>
  </label>
  <span class="lang-label" id="label-zh" style="color: #888;">中文</span>
</div>

<div class="lang-en" markdown="1">

# Curriculum Vitae

[Download My CV](/assets/pdf/CV-Jian.pdf)

## Education

* [2026.09 – 2031.07 (Expected)] PhD Student at [DBGroup@SZU](https://szu-dbgroup.github.io/), supervised by Prof. Dingming Wu, [CSSE](https://csse.szu.edu.cn/), [Shenzhen University](https://www.szu.edu.cn/) (SZU), China
* [2022.09 – 2026.07] B.Eng. in Computer Science and Technology (Outstanding Class), [CSSE](https://csse.szu.edu.cn/), [Shenzhen University](https://www.szu.edu.cn/) (SZU), China

## Publications
* Approximate DBSCAN via Density-Biased Sampling and Kernel Density Estimation, **SIGMOD 2026**.

## Honors (Selected)
* [2026] Top 100 Outstanding Bachelor's Theses, Class of 2026, Shenzhen University (Top 1.5%) 

## Scholarships & Awards (Selected)
* [2026] Integrated Bachelor–PhD Program Scholarship, Shenzhen University
* [2025] Second Prize, Top-notch Innovative Talent Scholarship, Shenzhen University
* [2024] Second Prize, Top-notch Innovative Talent Scholarship, Shenzhen University
* [2023] First Prize, Top-notch Innovative Talent Scholarship, Shenzhen University

</div>

<div class="lang-zh" style="display: none;" markdown="1">

# 个人简历

[下载我的简历](/assets/pdf/CV-Jian.pdf)

## 教育背景

* [2026.09 – 2031.07 (预计)] 博士研究生，[深圳大学数据库课题组 (DBGroup@SZU)](https://szu-dbgroup.github.io/)，导师：吴定明副教授，[计算机与软件学院](https://csse.szu.edu.cn/)，[深圳大学](https://www.szu.edu.cn/)
* [2022.09 – 2026.07] 工学学士，计算机科学与技术 (卓越班)，[计算机与软件学院](https://csse.szu.edu.cn/)，[深圳大学](https://www.szu.edu.cn/)

## 发表论文
* Approximate DBSCAN via Density-Biased Sampling and Kernel Density Estimation, **SIGMOD 2026**.

## 荣誉奖项 (部分)
* [2026] 深圳大学 2026 届百篇优秀本科毕业论文 (前 1.5%)

## 奖学金及奖项 (部分)
* [2026] 深圳大学本博一体化培养奖学金
* [2025] 深圳大学拔尖创新人才奖学金，二等奖
* [2024] 深圳大学拔尖创新人才奖学金，二等奖
* [2023] 深圳大学拔尖创新人才奖学金，一等奖

</div>

<style>
/* 容器样式：靠右对齐，垂直居中 */
.lang-toggle-container {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 12px;
  margin-bottom: 25px;
  font-family: inherit;
  font-weight: bold;
}

.lang-label {
  font-size: 0.9em;
  transition: color 0.3s ease;
}

/* 核心开关样式 */
.switch {
  position: relative;
  display: inline-block;
  width: 50px;
  height: 26px;
  margin: 0;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  transition: .4s;
}

.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}

.slider:before {
  position: absolute;
  content: "";
  height: 18px;
  width: 18px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  transition: .4s;
}

/* 开启状态 (切换到中文时的颜色) */
input:checked + .slider {
  background-color: #007bff; /* 可以根据你主页的色调修改这个颜色 */
}

input:focus + .slider {
  box-shadow: 0 0 1px #007bff;
}

input:checked + .slider:before {
  transform: translateX(24px);
}
</style>

<script>
function toggleLanguage() {
  var isChecked = document.getElementById('langSwitch').checked;
  var enElements = document.querySelectorAll('.lang-en');
  var zhElements = document.querySelectorAll('.lang-zh');
  var labelEn = document.getElementById('label-en');
  var labelZh = document.getElementById('label-zh');
  
  if (isChecked) {
    // 切换到中文
    enElements.forEach(el => el.style.display = 'none');
    zhElements.forEach(el => el.style.display = 'block');
    labelEn.style.color = '#888';       // 英文标签变灰
    labelZh.style.color = '#007bff';    // 中文标签高亮
  } else {
    // 切换回英文
    zhElements.forEach(el => el.style.display = 'none');
    enElements.forEach(el => el.style.display = 'block');
    labelZh.style.color = '#888';       // 中文标签变灰
    labelEn.style.color = '#007bff';    // 英文标签高亮
  }
}
</script>