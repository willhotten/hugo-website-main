---
title: "CV"
url: "/cv/"
date: 2023-07-14T01:11:12+01:00
draft: false
---

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
$(document).ready(function() {
  $(".tab_content").hide();
  $(".tabs li:first").addClass("active").show();
  $(".tab_content:first").show();

  $(".tabs li").click(function() {
    $(".tabs li").removeClass("active");
    $(this).addClass("active");
    $(".tab_content").hide();

    var activeTab = $(this).find("a").attr("href");
    $(activeTab).fadeIn();
    return false;
  });
});
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+3&display=swap');

.tabs {
  list-style-type: none;
  margin: 0;
  padding: 0;
  text-align: center;
  font-family: 'Source Sans 3', sans-serif;
}

.tabs li {
  display: inline-block;
  margin: 5px;
}

.tabs li a {
  display: block;
  padding: 10px;
  background-color: transparent;
  color: #333;
  text-decoration: none;
  border-radius: 50px;
}

.tabs li a:hover, .tabs li.active a {
  background-color: #ccc;
  font-weight: bold;
}

.tab_content {
  display: none;
  padding: 20px;
  background-color: transparent;
}

.education-item {
  margin-bottom: 20px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-family: 'Source Sans 3', sans-serif;
  background: transparent;
  position: relative;
}

.education-header {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.education-header img {
  width: 100px;
  height: 100px;
  margin-right: 20px;
}

.education-header div {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.education-item h3 {
  font-size: 20px;
  font-weight: bold;
  margin: 0;
  padding: 0;
  line-height: 1;
}

.education-item p {
  margin: 0;
  padding: 0;
  line-height: 1;
}

.download-button {
  display: block;
  width: 200px;
  margin: 0 auto;
  text-align: center;
  padding: 10px;
  border-radius: 20px;
  background-color: transparent;
  color: #333;
  text-decoration: none;
  font-family: 'Source Sans 3', sans-serif;
}

.download-button:hover {
  background-color: #333;
}
</style>

<ul class="tabs">
  <li class="active"><a href="#education">Education</a></li>
  <li><a href="#teaching">Teaching</a></li>
  <li><a href="#other_positions">Other Positions</a></li>
</ul>

<div class="tab_container">

<div id="education" class="tab_content">

  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg/1920px-RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg" alt="London Business School Logo">
      <div>
        <h3>London Business School</h3>
        <p>PhD in Economics</p>
        <p>2022 - Current</p>
        <p>Supervisor: Paolo Surico</p>
      </div>
    </div>
  </div>

  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/LSE_Logo.svg/638px-LSE_Logo.svg.png" alt="LSE Logo">
      <div>
        <h3>London School of Economics and Political Science</h3>
        <p>MSc in Economics</p>
        <p>2019 - 2020</p>
      </div>
    </div>
  </div>

  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/LSE_Logo.svg/638px-LSE_Logo.svg.png" alt="LSE Logo">
      <div>
        <h3>London School of Economics and Political Science</h3>
        <p>BSc in Economics</p>
        <p>2016 - 2019</p>
      </div>
    </div>
  </div>

</div>
</div>

<div id="teaching" class="tab_content">

  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg/1920px-RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg" alt="London Business School Logo">
      <div>
        <h3>London Business School</h3>
        <p>Teaching Assistant for P233 Macreoconomics II</p>
        <p>2024 - Current</p>
        <p>Instructor: Paolo Surico</p>
      </div>
    </div>
  </div>

</div>

<div id="other_positions" class="tab_content">

  <div class="education-item">
    <div class="education-header">
    <img src="https://cdn-ukwest.onetrust.com/logos/f79a60b0-1d16-4114-aa58-3f05dec13dd2/456b4352-7aaf-4e03-b3c8-439d63b7e437/0daef2ad-b42e-4bdc-8290-73d8f8f843da/PA_Logo_2022_800px.png" alt="PA Consulting Logo">
      <div>
        <h3>PA Consulting</h3>
        <p>Economist</p>
        <p>2021 - 2022</p>
      </div>
    </div>
  </div>

  <div class="education-item">
    <div class="education-header">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg/1920px-RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg" alt="London Business School Logo">
      <div>
        <h3>London Business School</h3>
        <p>Research Assistant to Hélène Rey and Vania Stavrakeva</p>
        <p>2020 - 2021</p>
      </div>
    </div>
  </div>

</div>


<a href="https://github.com/willhotten/CV/blob/677e6679bf4f5ad77df92865b7c68071880a36d9/CV%20Will%20Hotten.pdf" class="download-button">Download full CV</a>