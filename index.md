<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>The Momentum Reclaimer</title>
  <script src="https://unpkg.com/html2pdf.js"></script>
  <meta property="og:title" content="The Momentum Reclaimer" />
  <meta property="og:description" content="A self-guided workbook to reduce meeting bloat and reclaim deep work time—built for product teams and execs." />
  <meta property="og:image" content="social-preview.png" />
  <meta property="og:url" content="https://yonnastgetahun.github.io/momentum-audit-reclaimer/" />
  <meta name="twitter:card" content="summary_large_image" />
  <style>
    :root {
      --primary: #FF6B6B;
      --secondary: #1A1C33;
      --accent: #B5EAD7;
    }
    body {
      font-family: 'Helvetica Neue', sans-serif;
      background: var(--accent);
      color: var(--secondary);
      padding: 2rem;
      max-width: 800px;
      margin: auto;
      line-height: 1.6;
      position: relative;
    }
    h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
      color: var(--secondary);
    }
    h2 {
      font-size: 1.5rem;
      margin-top: 2rem;
      color: var(--secondary);
    }
    textarea, input[type="text"] {
      width: 100%;
      padding: 0.75rem;
      margin: 0.5rem 0 1.5rem;
      border: 1px solid var(--secondary);
      border-radius: 6px;
      font-size: 1rem;
      background: white;
      color: var(--secondary);
    }
    label {
      font-weight: bold;
      display: block;
      margin-top: 1rem;
      color: var(--secondary);
    }
    input[type="checkbox"] {
      margin-right: 0.5rem;
    }
    .btn {
      background-color: var(--primary);
      color: white;
      padding: 0.75rem 1.25rem;
      font-size: 1rem;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    .btn:hover {
      background-color: #e05555;
    }
    .section {
      background: white;
      padding: 2rem;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
      margin-bottom: 2rem;
    }
    .logo-top-right {
      position: fixed;
      top: 1rem;
      right: 1rem;
      max-width: 100px;
      z-index: 999;
    }
    .header-bar {
      position: sticky;
      top: 0;
      width: 100%;
      background: var(--accent);
      text-align: center;
      font-size: 1.2rem;
      font-weight: bold;
      padding: 0.75rem;
      border-bottom: 2px solid var(--secondary);
      z-index: 998;
    }
  </style>
</head>
<body>
  <div class="header-bar">The Momentum Reclaimer Workbook</div>
  <img src="pulse_collab_logo_large.png" alt="Pulse Collab Logo" class="logo-top-right" />
  <div id="audit-content">
    <div class="section">
      <h1>📘 The Momentum Reclaimer</h1>
      <p>A self-guided audit to help product teams and execs reduce meeting bloat and reclaim deep work time.</p>
    </div>
    <div style="text-align: center; margin-top: 3rem; font-size: 0.95rem;">
      <p>🔗 Visit <a href="https://pulsecollabagency.com/" target="_blank" style="color: var(--secondary); text-decoration: underline;">pulsecollabagency.com</a><br>
      📬 <a href="mailto:contact@pulsecollabagency.com" style="color: var(--secondary); text-decoration: underline;">contact us</a></p>
    </div>
    <div style="text-align: center; margin-top: 2rem;">
      <button class="btn" onclick="generatePDF()">📥 Download My Audit as PDF</button>
    </div>
  </div>
  <script>
    function generatePDF() {
      const element = document.getElementById("audit-content");
      html2pdf().from(element).save("momentum-reclaimer.pdf");
    }
  </script>
</body>
</html>



