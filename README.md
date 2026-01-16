# My-Index
รวบรวมเว็บที่จัดทำขึ้นเพื่อตรวจสอบในงาน
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Egis – Project Portal</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <style>
    body {
      font-family: "Segoe UI", Arial, sans-serif;
      background: #f4f6f8;
      margin: 0;
      color: #111111;
    }

    header {
      background: white;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 4px solid #8DC63F;
    }

    .logo-area {
      display: flex;
      align-items: center;
    }

    .logo-area img {
      height: 50px;
      margin-right: 20px;
    }

    .author {
      text-align: right;
      font-size: 13px;
      line-height: 1.4;
    }

    .linkedin {
      display: inline-block;
      margin-top: 6px;
      font-size: 13px;
      color: #8DC63F;
      text-decoration: none;
      font-weight: 500;
    }

    .container {
      max-width: 1000px;
      margin: 40px auto;
      padding: 20px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      border-radius: 10px;
      padding: 20px;
      border-top: 4px solid #8DC63F;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    }

    .card a {
      display: inline-block;
      margin-top: 12px;
      background: #8DC63F;
      color: white;
      padding: 10px 18px;
      border-radius: 6px;
      text-decoration: none;
    }

    footer {
      text-align: center;
      padding: 20px;
      font-size: 12px;
      color: #777;
    }

    /* Floating Download Button */
    .floating-download {
      position: fixed;
      bottom: 25px;
      right: 25px;
      background: #8DC63F;
      color: white;
      padding: 14px 20px;
      border-radius: 50px;
      font-weight: 600;
      text-decoration: none;
      box-shadow: 0 6px 15px rgba(0,0,0,0.2);
      z-index: 999;
    }

    /* Download Page (Hidden by default) */
    #download-page {
      display: none;
      padding: 40px;
    }

    .download-container {
      max-width: 800px;
      margin: auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .file-card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      border-top: 4px solid #8DC63F;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
    }

    .file-card a {
      display: inline-block;
      margin-top: 10px;
      background: #8DC63F;
      color: white;
      padding: 8px 16px;
      border-radius: 6px;
      text-decoration: none;
    }

    .back-btn {
      display: block;
      text-align: center;
      margin-top: 40px;
      color: #8DC63F;
      font-weight: 600;
      cursor: pointer;
    }
  </style>
</head>

<body>

<!-- HEADER -->
<header>
  <div class="logo-area">
    <img src="egis-logo.png" alt="Egis Logo">
    <div>
      <h1>Egis – Project Portal</h1>
      <p>BIM & Digital Engineering Tools</p>
    </div>
  </div>

  <div class="author">
    <strong>Prepared by:</strong><br>
    Nook (Dararat Poungmalee)<br>
    <span>BIM / Digital Engineer</span><br>
    <a href="https://www.linkedin.com/in/dararat-p-89719a182" target="_blank" class="linkedin">
      LinkedIn Profile
    </a>
  </div>
</header>

<!-- MAIN PAGE -->
<div id="main-page">

  <div class="container">

    <div class="card">
      <h3>BIM Record Revision</h3>
      <p>Record revision history for Fab Sheet submissions.</p>
      <a href="https://dararat28.github.io/INH_Record_Revision/" target="_blank">Open Project</a>
    </div>

    <div class="card">
      <h3>Check Code-Duplicates</h3>
      <p>Detect duplicate codes in the system.</p>
      <a href="https://dararat28.github.io/INH-Check-Code-Duplicates-/" target="_blank">Open Project</a>
    </div>

    <div class="card">
      <h3>Check-Height Code</h3>
      <p>Manage height data for each code.</p>
      <a href="https://dararat28.github.io/INH_Check-Height/" target="_blank">Open Project</a>
    </div>

    <div class="card">
      <h3>PDF Ticket Checker</h3>
      <p>Verify elevation and quantities from Revit.</p>
      <a href="https://dararat28.github.io/PDF-Ticket-Checker/" target="_blank">Open Project</a>
    </div>

    <div class="card">
      <h3>PDF Schedule Excel Checker</h3>
      <p>Compare PDF schedules with Revit Excel quantities.</p>
      <a href="https://dararat28.github.io/PDF-Excel-Checker/" target="_blank">Open Project</a>
    </div>

  </div>
</div>

<!-- DOWNLOAD PAGE -->
<div id="download-page">

  <h2 style="text-align:center;">Download BIM / Dynamo Tools</h2>

  <div class="download-container">

    <div class="file-card">
      <h3>Template_Delete_file Cad_import</h3>
      <a href="downloads/Template_Delete_file Cad_import.dyn" download>Download</a>
    </div>

    <div class="file-card">
      <h3>Dynamo for Export Element ID to Excel</h3>
      <a href="downloads/Dynamo for Export Element ID to Excel.dyn" download>Download</a>
    </div>

    <div class="file-card">
      <h3>LinkDWG</h3>
      <a href="downloads/LinkDWG.dyn" download>Download</a>
    </div>

     <div class="file-card">
      <h3>Convert Cad Block to Family</h3>
      <a href="downloads/Convert Cad Block to Family.dyn" download>Download</a>
    </div>

  </div>

  <div class="back-btn" onclick="showMain()">← Back to Main Page</div>
</div>

<!-- Floating Button -->
<a class="floating-download" onclick="showDownload()">⬇ Download Tools</a>

<footer>
  © 2026 Egis | Digital Engineering Projects
</footer>

<script>
  function showDownload() {
    document.getElementById("main-page").style.display = "none";
    document.getElementById("download-page").style.display = "block";
  }

  function showMain() {
    document.getElementById("download-page").style.display = "none";
    document.getElementById("main-page").style.display = "block";
  }
</script>

</body>
</html>
