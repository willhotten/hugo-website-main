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
.tabs {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.tabs li {
  display: inline-block;
  margin-right: 10px;
}

.tabs li a {
  display: block;
  padding: 10px;
  background-color: #f2f2f2;
  color: #333;
  text-decoration: none;
}

.tabs li a:hover {
  background-color: #ccc;
}

.tab_content {
  display: none;
  padding: 20px;
  background-color: #f2f2f2;
}
</style>

<ul class="tabs">
  <li class="active"><a href="#education">Education</a></li>
  <li><a href="#teaching">Teaching</a></li>
  <li><a href="#other_positions">Other Positions</a></li>
  <li><a href="#stipends_awards">Stipends and Awards</a></li>
  <li><a href="#computer_skills">Computer Skills</a></li>
</ul>

<div class="tab_container">
  <div id="education" class="tab_content">
    ##London Business School - PhD in Economics (2022 ‑ Current)

    - 2nd year PhD student in the Economics department
    - Supervisor: Paolo Surico
    - Research interests: Inequality, Heterogeneity in Macroeconomics, Financial Macroeconomics, Climate Policy

    ## London School of Economics and Political Science - MSc in Economics (2019 ‑ 2020)

    - Grade: Distinction
    - Courses: Microeconomics, Macroeconomics, Econometrics, Monetary Economics

    ## London School of Economics and Political Science - BSc in Economics (2016 ‑ 2019)

    - Grade: First‑Class Honours
    - Electives: Advanced Economic Analysis, International Economics, Industrial Economics, Monetary Economics
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

  <div id="stipends_awards" class="tab_content">
    ## London Business School - PhD stipend (2022 - 2027)
  </div>

  <div id="computer_skills" class="tab_content">
    Programming: MATLAB, Python, R, Stata
    Miscellaneous: LATEX, Microsoft Office, Git., Bloomberg, Refinitiv Eikon
  </div>

<style>
.download-button {
  display: block;
  width: 200px;
  margin: 0 auto;
  text-align: center;
  padding: 10px;
  border-radius: 20px;
  background-color: #333;
  color: #fff;
  text-decoration: none;
}

.download-button:hover {
  background-color: #555;
}
</style>

<a href="https://github.com/willhotten/CV/blob/677e6679bf4f5ad77df92865b7c68071880a36d9/CV%20Will%20Hotten.pdf" class="download-button">Download CV</a>