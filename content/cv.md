---
title: "CV"
url: "/cv/"
date: 2023-07-14T01:11:12+01:00
draft: false
---

<html>

<head>

 <title>Adobe Acrobat Services PDF Embed API Sample</title>

 <meta charset="utf-8"/>

 <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/>

 <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1"/>

</head>

<body style="margin: 0px">

 <div id="adobe-dc-view"></div>

 <script src="https://acrobatservices.adobe.com/view-sdk/viewer.js"></script>

 <script type="text/javascript">

    document.addEventListener("adobe_dc_view_sdk.ready", function()

    {

        var adobeDCView = new AdobeDC.View({clientId: "d5c0ca8bef754aecb5f40f45d47c0e90", divId: "adobe-dc-view"});

        adobeDCView.previewFile(

       {

          content:   {location: {url: "https://github.com/willhotten/CV/blob/main/CV%20Will%20Hotten.pdf"}},

          metaData: {fileName: "CV_Will_Hotten.pdf"}

       });

    });

 </script>

</body>

</html>

<div id="adobe-dc-view" style="height: 360px; width: 500px;"></div>

<script src="https://acrobatservices.adobe.com/view-sdk/viewer.js"></script>

<script type="text/javascript">

  document.addEventListener("adobe_dc_view_sdk.ready", function(){

    var adobeDCView = new AdobeDC.View({clientId: "<d5c0ca8bef754aecb5f40f45d47c0e90>", divId: "adobe-dc-view"});

    adobeDCView.previewFile({

      content:{location: {url: "https://acrobatservices.adobe.com/view-sdk-demo/PDFs/Bodea Brochure.pdf"}},

      metaData:{fileName: "Bodea Brochure.pdf"}

    }, { embedMode: "SIZED_CONTAINER", showFullScreen: true });

  });

</script>