+++
title = "CV"
layout = "single"
url = "/cv/"
+++

<div class="cv-header">
  <h1>Curriculum Vitae</h1>
</div>

<div class="cv-tabs">
  <button class="tab active" data-tab="education">Education</button>
  <button class="tab" data-tab="teaching">Teaching</button>
  <button class="tab" data-tab="positions">Other Positions</button>
</div>

<div class="cv-tab-content active" id="education">
  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg/1920px-RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg" alt="London Business School Logo">
      <div>
        <h3>London Business School</h3>
        <p>PhD in Economics</p>
        <p>2022 – Current</p>
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
        <p>2019 – 2020</p>
      </div>
    </div>
  </div>

  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/LSE_Logo.svg/638px-LSE_Logo.svg.png" alt="LSE Logo">
      <div>
        <h3>London School of Economics and Political Science</h3>
        <p>BSc in Economics</p>
        <p>2016 – 2019</p>
      </div>
    </div>
  </div>
</div>

<div class="cv-tab-content" id="teaching">
  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg/1920px-RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg" alt="London Business School Logo">
      <div>
        <h3>London Business School</h3>
        <p>Teaching Assistant for P233 Macroeconomics II</p>
        <p>2024 – Current</p>
        <p>Instructor: Paolo Surico</p>
      </div>
    </div>
  </div>
</div>

<div class="cv-tab-content" id="positions">
  <div class="education-item">
    <div class="education-header">
      <img src="https://cdn-ukwest.onetrust.com/logos/f79a60b0-1d16-4114-aa58-3f05dec13dd2/456b4352-7aaf-4e03-b3c8-439d63b7e437/0daef2ad-b42e-4bdc-8290-73d8f8f843da/PA_Logo_2022_800px.png" alt="PA Consulting Logo">
      <div>
        <h3>PA Consulting</h3>
        <p>Economist</p>
        <p>2021 – 2022</p>
      </div>
    </div>
  </div>

  <div class="education-item">
    <div class="education-header">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg/1920px-RS9327_LBS_Standard_Logo_RGB_AW-hpr.jpg" alt="London Business School Logo">
      <div>
        <h3>London Business School</h3>
        <p>Research Assistant to Hélène Rey and Vania Stavrakeva</p>
        <p>2020 – 2021</p>
      </div>
    </div>
  </div>
</div>

<a href="https://github.com/willhotten/CV/blob/677e6679bf4f5ad77df92865b7c68071880a36d9/CV%20Will%20Hotten.pdf" class="download-button">Download full CV</a>

<script>
  document.querySelectorAll('.tab').forEach(button => {
    button.addEventListener('click', () => {
      document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
      document.querySelectorAll('.cv-tab-content').forEach(c => c.classList.remove('active'));
      button.classList.add('active');
      document.getElementById(button.dataset.tab).classList.add('active');
    });
  });
</script>