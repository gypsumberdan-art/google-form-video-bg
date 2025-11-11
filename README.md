<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Google Form with Video Background</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden;
      font-family: Arial, sans-serif;
    }
    video {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
    }
    iframe {
      position: relative;
      width: 100%;
      height: 100vh;
      border: none;
      z-index: 1;
      background-color: rgba(255, 255, 255, 0.85); /* optional: slightly transparent white background */
      backdrop-filter: blur(4px);
    }
  </style>
</head>
<body>
  <video autoplay muted loop playsinline>
    <source src=https://drive.google.com/file/d/1R-8XQNSIoHmZYunHOrxYbLXFFcWg41PO/view?usp=drive_linktype="video/mp4">
  </video>

  <iframe src=https://docs.google.com/forms/d/e/1FAIpQLScKEc9Ln631ncUvF8-huQsZR9jfTHTB54559MwacmMEd0_14Q/viewform?usp=dialog></iframe>
</body>
</html>
