<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Cybercrime Project File</title>
  <style>
    body {
      font-family: "Segoe UI", sans-serif;
      background: #000;
      margin: 0;
      padding: 20px;
      color: #fff;
      overflow-x: hidden;
    }

    /* Falling binary effect */
    canvas {
      position: fixed;
      top: 0;
      left: 0;
      z-index: -1;
    }

    .page {
      width: 800px;
      margin: 30px auto;
      padding: 55px;
      background: rgba(17, 17, 17, 0.9);
      border: 2px solid #00e5ff;
      border-radius: 10px;
      box-shadow: 0 0 20px rgba(0,229,255,0.6);
      position: relative;
    }

    h1, h2, h3 {
      text-align: center;
      color: #00e5ff;
    }
    .title {
      font-size: 40px;
      color: #ffea00;
      text-transform: uppercase;
      letter-spacing: 2px;
      text-shadow: 0 0 8px #ffea00;
    }
    .subtitle {
      text-align: center;
      font-size: 18px;
      margin-top: -10px;
      color: #bbb;
    }
    .slogan {
      font-size: 24px;
      text-align: center;
      color: #ff1744;
      text-shadow: 0 0 8px #ff1744;
      margin: 20px 0;
    }
    .list {
      margin-left: 40px;
      font-size: 18px;
      color: #ddd;
    }
    a {
      color: #00e5ff;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .footer {
      text-align: right;
      margin-top: 40px;
      font-size: 14px;
      color: #888;
    }
    img {
      display: block;
      margin: 20px auto;
      width: 80%;
      border: 2px solid #00e5ff;
      border-radius: 10px;
      box-shadow: 0 0 15px #00e5ff;
    }
  </style>
</head>
<body>

  <!-- Falling Matrix Effect -->
  <canvas id="matrix"></canvas>
  <script>
    const canvas = document.getElementById("matrix");
    const ctx = canvas.getContext("2d");

    canvas.height = window.innerHeight;
    canvas.width = window.innerWidth;

    const binary = "01";
    const font_size = 16;
    const columns = canvas.width / font_size;

    const drops = [];
    for (let x = 0; x < columns; x++) drops[x] = 1;

    function draw() {
      ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
      ctx.fillRect(0, 0, canvas.width, canvas.height);

      ctx.fillStyle = "#0F0"; // Green binary
      ctx.font = font_size + "px monospace";

      for (let i = 0; i < drops.length; i++) {
        const text = binary[Math.floor(Math.random() * binary.length)];
        ctx.fillText(text, i * font_size, drops[i] * font_size);

        if (drops[i] * font_size > canvas.height && Math.random() > 0.975)
          drops[i] = 0;
        drops[i]++;
      }
    }
    setInterval(draw, 33);

    // Resize handler
    window.addEventListener("resize", () => {
      canvas.height = window.innerHeight;
      canvas.width = window.innerWidth;
    });
  </script>


</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Cybercrime Project File</title>
  <style>
    body 
    {
     
      font-family: "Segoe UI", sans-serif;
      background: #000;
      margin: 0;
      padding: 20px;
      color: #fff;
    }

    .page {
      width: 800px;
      margin: 30px auto;
      padding: 40px;
      background: #070707;
      border: 2px solid #00b7ff;
      border-radius: 10px;
      box-shadow: 0 0 30px rgba(0,229,255,0.6);
    }
    h1, h2, h3 {
      text-align: center;
      color: #00e5ff;
      text-shadow: 0 0 10px #ff0d0d;
    }
    .title {
      font-size: 36px;
      color: #ffea00;
      text-transform: uppercase;
      letter-spacing: 2px;
      text-shadow: 0 0 12px #ffea00;
    }
    .subtitle {
      text-align: center;
      font-size: 18px;
      margin-top: -10px;
      color: #bbb;
    }
    .slogan {
      font-size: 24px;
      text-align: center;
      color: #ff1744;
      text-shadow: 0 0 8px #ff1744;
      margin: 20px 0;
    }
    .list {
      margin-left: 40px;
      font-size: 18px;
      color: #ddd;
    }
    a {
      color: #00e5ff;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .footer {
      text-align: right;
      margin-top: 40px;
      font-size: 14px;
      color: #888;
    }
    img {
      display: block;
      margin: 20px auto;
      width: 80%;
      border: 2px solid #00e5ff;
      border-radius: 10px;
      box-shadow: 0 0 15px #00e5ff;
    }

   #matrixCanvas {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -1; /* behind text */
    }

    .content {
      position: relative;
      z-index: 1; /* on top of falling code */
      padding: 20px;
      text-align: center;
    }
  </style>
</head>
<body>

  <!-- Page 1: Cover -->
  <div class="page">
    <h1 class="title">Cyber Crime</h1>
    <p class="subtitle">A Project on Digital Threats & Security</p>
    <p style="text-align:center; font-size:24px;">📱💻🔒</p>
  </div>

  <!-- Page 2: Certificate -->
  <div class="page">
    <h2>Certificate</h2>
    <p>This is to certify that the project work entitled <b>“Cyber Crime – Digital Threats & Security”</b> has been successfully completed by our group during the academic year 2025–26.</p>
    <p>This project is submitted in partial fulfillment of Information Technology subject requirements.</p>
    <br><br>
    <p>name of teacher--miss sakshi bhandari✨</p>
    <p></p>
  </div>

  <!-- Page 3: Acknowledgment -->
  <div class="page">
    <h2>Acknowledgment</h2>
    <p>We would like to express our sincere gratitude to our respected teacher <b>Miss Sakshi Bhandari</b> for her guidance, encouragement, and valuable suggestions throughout this project.</p>
    <p>We also thank our school principal and our classmates for their constant support.</p>
  </div>

  <!-- Page 4–6: Group Photos -->
  <div class="page">
    <h2>Group Photo</h2>
    <img src="89328561-e713-49cd-a2a8-70bc690e3d2d.png" alt="Group Photo 1">
  </div>

  <div class="page">
    <h2>Group Photo</h2>
    <img src"" alt="Group Photo 2">
  </div>

  <div class="page">
    <h2>fie cover</h2>
    <img src="C:\Users\hp\Documents\old\cover.webp" alt="Laptop Photo">
  </div>

  <!-- Page 7: Member Names -->
  <div class="page">
    <h2>Group Members 👥</h2>
    <div class="list">
      <p>1. Chinmay Sati</p>
      <p>2. Ayush Bhatt</p>
      <p>3. Arush Sati</p>
      <p>4. Ankit Pardali</p>
      <p>5. Aryan Jawan</p>
      <p>6. Naitik Thaplyal</p>
    </div>
    <br>
    <p><b>Submitted To:</b> Miss Sakshi Bhandari ✨</p>
  </div>

  <!-- Page 8: Index -->
  <div class="page">
    <h2>Index</h2>
    <ol>
      <li>Cover Page</li>
      <li>Certificate</li>
      <li>Acknowledgment</li>
      <li>Group Photos</li>
      <li>Member Names</li>
      <li>Index</li>
      <li>Introduction</li>
      <li>Slogans</li>
      <li>Types of Cybercrime</li>
      <li>Cyber Laws in India</li>
      <li>International Cyber Laws</li>
      <li>Cybersecurity Measures</li>
      <li>Case Studies</li>
      <li>Future of Cybercrime & Conclusion</li>
      <li>Bibliography</li>
      <li>Back Cover</li>
    </ol>
  </div>

  <!-- Page 9: Introduction -->
  <div class="page">
    <h2>Introduction</h2>
    <p>The internet has become the backbone of our lives, but with advantages come threats. <b>Cybercrime</b> refers to illegal activities using computers, networks, or the internet. This project highlights types of cybercrime, laws, and measures to prevent them.</p>
  </div>

  <!-- Page 10–12: Slogans -->
  <div class="page"><p class="slogan">Think Before You Click 👆</p></div>
  <div class="page"><p class="slogan">Prevention is Better than Recovery 🔐</p></div>
  <div class="page"><p class="slogan">Your Password is Your Key – Don’t Share It 🔑</p></div>

  <!-- Page 13: Types of Cybercrime (1) -->
  <div class="page">
    <h2>Types of Cybercrime (1)</h2>
    <ul class="list">
      <li><b>Hacking</b> – Unauthorized access to systems.</li>
      <li><b>Phishing</b> – Fake messages to steal personal data.</li>
    </ul>
  </div>

  <!-- Page 14: Types of Cybercrime (2) -->
  <div class="page">
    <h2>Types of Cybercrime (2)</h2>
    <ul class="list">
      <li><b>Cyberbullying</b> – Online harassment.</li>
      <li><b>Malware</b> – Viruses, worms, ransomware.</li>
    </ul>
  </div>

  <!-- Page 15: Cyber Laws in India -->
  <div class="page">
    <h2>Cyber Laws in India</h2>
    <ul class="list">
      <li><b>IT Act 2000</b> – First law against cybercrimes.</li>
      <li><b>Punishments</b>:
        <ul>
          <li>Identity theft: Up to 3 years jail + fine.</li>
          <li>Hacking: Up to 3 years jail + ₹5 lakh fine.</li>
        </ul>
      </li>
    </ul>
  </div>

  <!-- Page 16: International Cyber Laws -->
  <div class="page">
    <h2>International Cyber Laws</h2>
    <ul class="list">
      <li><b>Budapest Convention on Cybercrime</b></li>
      <li><b>Global cooperation</b> to fight cross-border crimes.</li>
    </ul>
  </div>

  <!-- Page 17: Cybersecurity Measures -->
  <div class="page">
    <h2>Cybersecurity Measures</h2>
    <h3>For Individuals</h3>
    <ul class="list">
      <li>Strong passwords</li>
      <li>Two-factor authentication</li>
      <li>Antivirus software</li>
      <li>Awareness</li>
    </ul>
    <h3>For Organizations</h3>
    <ul class="list">
      <li>Firewalls</li>
      <li>Employee training</li>
      <li>Data backups</li>
    </ul>
  </div>

  <!-- Page 18: Case Studies -->
  <div class="page">
    <h2>Case Studies</h2>
    <h3>India</h3>
    <p>2016 SBI phishing scam – millions lost.</p>
    <h3>World</h3>
    <p>WannaCry ransomware 2017 – 150+ countries affected.</p>
  </div>

  <!-- Page 19: Future & Conclusion -->
  <div class="page">
    <h2>Future of Cybercrime & Conclusion</h2>
    <p>Future threats: AI-driven scams, deepfakes, IoT hacks.  
    But awareness, strict laws, and global cooperation can keep us safe.</p>
    <p><b>Conclusion:</b> Cybersecurity is not optional—it’s essential.</p>
  </div>

  <!-- Page 20: Bibliography & Back Cover -->
  <div class="page">
    <h2>Bibliography / References</h2>
    <ul class="list">
      <li>NCERT Information Technology Book</li>
      <li><a href="https://www.cert-in.org.in" target="_blank">https://www.cert-in.org.in</a></li>
      <li>Various news articles and journals</li>
    </ul>
  </div>
  <div class="page">
    <h2>CREATED BY CHINMAY SATI</h2>
    <ul class="list">
      <li>for seva project file</li>
      <li>woth suppor of group member who take my work and give me time to make it</li>
      <li>we have work hard for this project i hope for getting 5 marks and aso hope you will ignore the img in file thankx</li>
    </ul>
    <div class="footer">Back Cover</div>
  </div>

  </script>

</body>
</html>

