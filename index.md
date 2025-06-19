<center>
  <h1>Perceptually-Guided VR Style Transfer</h1>
</center>
<center>
  <h2>Seonghwa Choi<sup>1</sup>, Jungwoo Huh<sup>1</sup>, Sanghoon Lee<sup>1*</sup>, and Alan Conrad Bovik<sup>2</sup> </h2>
</center>
<center>
  <h4><sup>1</sup> Yonsei University, Korea &emsp; <sup>2</sup> The University of Texas at Austin, USA</h4>
</center>
<center>
  <h4><sup>*</sup> Indicates Corresponding Author</h4>
</center>

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
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
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
  <h3>Video Comparison</h3>
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
