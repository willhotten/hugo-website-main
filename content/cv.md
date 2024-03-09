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
  background: #fff;
  position: relative;
}

.education-header {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.education-header img {
  width: 75px;
  height: 75px;
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
}

.education-item p {
  margin: 0;
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
  background-color: #555;
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
</div>

<div id="teaching" class="tab_content">
    ## London Business School - Teaching assistant for P233 Macroeconomics II (PhD)
    
    - Advanced course in macroeconomics for PhD students, instructed by Paolo Surico
</div>

<div id="other_positions" class="tab_content">
    ## PA Consulting London - Economist (2021 ‑ 2022)

    ## London Business School - Research Assistant to Hélène Rey and Vania Stavrakeva (2020 ‑ 2021)

    ## Volunteering - Various: 

    - Career Ready, Mentor
    - Citizens Advice Basingstoke, Gateway Assessor
    - Action Tutoring, Maths Tutor
</div>


<a href="https://github.com/willhotten/hugo-website-main/blob/c4bfa6fa9845aafb090605ef1b5c02bda3ed0b56/pdfs/CV%20Will%20Hotten.pdf" class="download-button">Download full CV</a>