---
title: "CV"
url: "/cv/"
date: 2023-07-14T01:11:12+01:00
draft: false
---

Coming soon!

<div id="adobe-dc-view" style="height: 360px; width: 500px;"></div>

<script src="https://acrobatservices.adobe.com/view-sdk/viewer.js"></script>

<script type="text/javascript">

  document.addEventListener("adobe_dc_view_sdk.ready", function(){

    var adobeDCView = new AdobeDC.View({clientId: "<YOUR_CLIENT_ID>", divId: "adobe-dc-view"});

    adobeDCView.previewFile({

      content:{ location:

        { url: "https://github.com/willhotten/CV/blob/main/CV%20Will%20Hotten.pdf"}},

      metaData:{fileName: "Bodea Brochure.pdf"}

    },

    {

      embedMode: "SIZED_CONTAINER"

    });

  });

</script>