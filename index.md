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
    .logo {
      display: block;
      margin: 0 auto 1.5rem;
      max-width: 180px;
    }
  </style>
</head>
<body>
  <div id="audit-content">
    <img src="pulse_collab_logo_large.png" alt="Pulse Collab Logo" class="logo" />
    <div class="section">
      <h1>📘 The Momentum Reclaimer</h1>
      <p>A self-guided audit to help product teams and execs reduce meeting bloat and reclaim deep work time.</p>
    </div>
    <div class="section"><h2>Section 1: Your Context</h2><label for="role">Your Role & Responsibilities</label><textarea id="role"></textarea><label for="teamSize">Team Size</label><input type="text" id="teamSize" /><label for="deepWork">Weekly Deep Work Needs</label><textarea id="deepWork"></textarea><label for="frustrations">Biggest Meeting Frustration</label><textarea id="frustrations"></textarea></div>
    <div class="section"><h2>Section 2: Top 5 Recurring Meetings</h2><textarea id="meetings" rows="5"></textarea></div>
    <div class="section"><h2>Section 3: Quick Self-Check</h2><label><input type="checkbox" /> I lead most of these meetings</label><label><input type="checkbox" /> I attend but don’t contribute in half</label><label><input type="checkbox" /> I often multitask in meetings</label><label><input type="checkbox" /> I struggle to find focus time</label></div>
    <div class="section"><h2>Section 4: Make Cuts</h2><label for="eliminate">Meetings to Eliminate</label><textarea id="eliminate"></textarea><label for="reduce">Meetings to Reduce</label><textarea id="reduce"></textarea><label for="convert">Meetings to Convert to Async</label><textarea id="convert"></textarea><label for="combine">Meetings to Combine</label><textarea id="combine"></textarea></div>
    <div class="section"><h2>Section 5: Reclaim the Time</h2><label for="weekly">Time Reclaimed (per week)</label><input type="text" id="weekly" /><label for="monthly">Time Reclaimed (per month)</label><input type="text" id="monthly" /><label for="yearly">Time Reclaimed (per year)</label><input type="text" id="yearly" /><label for="reallocation">Where will you reinvest that time?</label><textarea id="reallocation"></textarea></div>
    <div class="section"><h2>Section 6: New Rules of Engagement</h2><label for="runRules">Rules for Meetings You Run</label><textarea id="runRules"></textarea><label for="attendRules">Rules for Meetings You Attend</label><textarea id="attendRules"></textarea><label for="zones">Protected Zones</label><textarea id="zones"></textarea></div>
    <div class="section"><h2>Section 7: Executive Summary</h2><label for="summaryWins">Top Wins / Calendar Changes</label><textarea id="summaryWins"></textarea><label for="impact">Team Impact / Morale Change</label><textarea id="impact"></textarea><label for="roi">Estimated ROI or Time Saved</label><textarea id="roi"></textarea><label for="nextSteps">Recommended Next Steps</label><textarea id="nextSteps"></textarea></div>
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


