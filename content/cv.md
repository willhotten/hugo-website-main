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
    ## Degree Name - University Name (Year)

    - Brief description of your degree program
    - Relevant coursework or projects
  </div>

  <div id="teaching" class="tab_content">
    ## Course Name - University Name (Year)

    - Description of your role as a teaching assistant or instructor
    - Responsibilities and accomplishments
  </div>

  <div id="other_positions" class="tab_content">
    ## Internship - Company Name (Year)

    - Description of your role and responsibilities
    - Key achievements or projects
  </div>

  <div id="stipends_awards" class="tab_content">
    - Award 1: Description of the award and its significance (Year)
    - Award 2: Description of the award and its significance (Year)
    - Award 3: Description of the award and its significance (Year)
  </div>

  <div id="computer_skills" class="tab_content">
    - Skill 1: Description of your proficiency level and relevant experience
    - Skill 2: Description of your proficiency level and relevant experience
    - Skill 3: Description of your proficiency level and relevant experience
  </div>

</body>

</html>

<div id="adobe-dc-view" style="height: 360px; width: 500px;"></div>

<script src="https://acrobatservices.adobe.com/view-sdk/viewer.js"></script>

<script type="text/javascript">

  document.addEventListener("adobe_dc_view_sdk.ready", function(){

    var adobeDCView = new AdobeDC.View({clientId: "d5c0ca8bef754aecb5f40f45d47c0e90", divId: "adobe-dc-view"});

    adobeDCView.previewFile({

      content:{location: {url: "https://blobby.wsimg.com/go/d9de11f7-2353-4193-a579-9de67e73890f/Coming-Soon.pdf"}},

      metaData:{fileName: "CV Will Hotten.pdf"}

    }, { embedMode: "LIGHT_BOX", showFullScreen: true });

  });

</script>