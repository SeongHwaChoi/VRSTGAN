# <center> Perceptually-Guided VR Style Transfer </center>
#### <center> Seonghwa Choi$^{1}$, Jungwoo Huh$^{1}$, Sanghoon Lee$^{1}$$^{*}$, and Alan Conrad Bovik </center>
<center> $^{1}$ Yonsei University, Korea $^{2}$ The University of Texas at Austin, USA </center>
<center> $^{*}$ Indicates Corresponding Author </center>


<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Video Comparison</title>
  <style>
    body {
      background: #fff;
      margin: 2rem;
      font-family: sans-serif;
    }
    .set {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 10px;
      margin-bottom: 50px;
    }
    .video-slot, .image-slot {
      background: #000;
      position: relative;
      width: 100%;
      padding-top: 56.25%; /* 16:9 ratio */
    }
    .video-slot video, .image-slot img {
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      object-fit: cover;
    }
    .label {
      text-align: center;
      margin-top: 0.5rem;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <center>
    <h1>Simple Video Display Grid</h1>
  </center>


  <div class="set">
    <div>
      <div class="image-slot"><img src="demo/style/00000106_(3).jpg" alt="Reference Image 1"></div>
      <div class="label">Style</div>
    </div>
    <div>
      <div class="video-slot"><video src="demo/ref/converted_vid1.mp4" autoplay loop muted></video></div>
      <div class="label">Content</div>
    </div>
  </div>
  <div class="set">
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/GCT.mp4" autoplay loop muted></video></div><div class="label">GCT</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/IDT.mp4" autoplay loop muted></video></div><div class="label">IDT</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/DeepColor.mp4" autoplay loop muted></video></div><div class="label">DeepColor</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/DSTN.mp4" autoplay loop muted></video></div><div class="label">DSTN</div></div>
  </div>
  <div class="set">
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/PhotoWCT2.mp4" autoplay loop muted></video></div><div class="label">PhotoWCT2</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/PKD.mp4" autoplay loop muted></video></div><div class="label">PKD</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/CCPL.mp4" autoplay loop muted></video></div><div class="label">CCPL</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/CAPVST.mp4" autoplay loop muted></video></div><div class="label">CAPVST</div></div>
    <div><div class="video-slot"><video src="demo/case1/00000106_(3)/Ours_ver2_ebgan.mp4" autoplay loop muted></video></div><div class="label">Ours</div></div>
  </div>

  <div class="set">
    <div>
      <div class="image-slot"><img src="demo/style/00000087_(2).jpg" alt="Reference Image 1"></div>
      <div class="label">Style</div>
    </div>
    <div>
      <div class="video-slot"><video src="demo/ref/G1Aerial.mp4" autoplay loop muted></video></div>
      <div class="label">Content</div>
    </div>
  </div>
  <div class="set">
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/GCT.mp4" autoplay loop muted></video></div><div class="label">GCT</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/IDT.mp4" autoplay loop muted></video></div><div class="label">IDT</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/DeepColor.mp4" autoplay loop muted></video></div><div class="label">DeepColor</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/DSTN.mp4" autoplay loop muted></video></div><div class="label">DSTN</div></div>
  </div>
  <div class="set">
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/PhotoWCT2.mp4" autoplay loop muted></video></div><div class="label">PhotoWCT2</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/PKD.mp4" autoplay loop muted></video></div><div class="label">PKD</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/CCPL.mp4" autoplay loop muted></video></div><div class="label">CCPL</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/CAPVST.mp4" autoplay loop muted></video></div><div class="label">CAPVST</div></div>
    <div><div class="video-slot"><video src="demo/case2/00000087_(2)/Ours_ver2_ebgan.mp4" autoplay loop muted></video></div><div class="label">Ours</div></div>
  </div>

<script>
  const videos = document.querySelectorAll('video');
  videos.forEach(v => v.playbackRate = 0.75);
</script>
</body>
</html>
