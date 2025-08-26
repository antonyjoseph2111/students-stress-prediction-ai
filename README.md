<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Stress Level Classification Model — Project Showcase</title>

  <!-- Fonts & Icons -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <link rel="icon" href="https://raw.githubusercontent.com/favicon.ico" />

  <!-- Simple Styling -->
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#98a0b3;
      --accent:#7c3aed;
      --glass: rgba(255,255,255,0.03);
      --glass-2: rgba(255,255,255,0.02);
      --white: #e6eef8;
    }
    *{box-sizing:border-box}
    body{
      margin:0; font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background: linear-gradient(180deg,#071022 0%, #07162a 60%); color:var(--white);
      -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
    }
    .container{max-width:980px;margin:40px auto;padding:28px;}
    .card{
      background:linear-gradient(180deg,var(--card), rgba(11,18,32,0.9));
      border-radius:14px; padding:28px; box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      border:1px solid rgba(255,255,255,0.03);
    }
    .header{display:flex;gap:18px;align-items:center}
    .logo{
      width:84px;height:84px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#e11d48);
      display:flex;align-items:center;justify-content:center;font-weight:700;font-size:34px;color:white;
      box-shadow:0 6px 24px rgba(124,58,237,0.25);
    }
    h1{margin:0;font-weight:700;font-size:28px}
    p.lead{color:var(--muted);margin-top:6px;margin-bottom:18px}
    .badges img{height:30px;margin-right:8px;border-radius:6px}
    .hero-gif{display:block;margin:18px auto;border-radius:12px;border:1px solid rgba(255,255,255,0.03)}
    .grid{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:20px}
    .box{background:var(--glass);border-radius:12px;padding:16px;border:1px solid var(--glass-2)}
    .section-title{font-weight:600;margin-bottom:8px;color:var(--white)}
    pre{background:#071022;padding:14px;border-radius:8px;overflow:auto;border:1px solid rgba(255,255,255,0.03);color:#bfe3ff}
    code{font-family:SFMono-Regular,Monaco,Consolas,"Liberation Mono",monospace;font-size:13px}
    ul{margin:8px 0 0 18px;color:var(--muted)}
    .btn{
      display:inline-block;padding:10px 14px;border-radius:10px;text-decoration:none;color:white;
      background:linear-gradient(90deg,var(--accent),#ef4444);font-weight:600;box-shadow:0 8px 20px rgba(124,58,237,0.18)
    }
    .muted{color:var(--muted);font-size:14px}
    .small{font-size:13px;color:var(--muted)}
    .repo-structure{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent); padding:12px;border-radius:10px}
    .footer{margin-top:22px;padding-top:18px;border-top:1px dashed rgba(255,255,255,0.03);color:var(--muted);font-size:14px}
    .stats{display:flex;gap:12px;flex-wrap:wrap;margin-top:12px}
    .stat{background:linear-gradient(90deg, rgba(255,255,255,0.02), transparent);padding:10px;border-radius:8px;min-width:110px}
    .gif-wrap{display:flex;gap:8px;flex-direction:column;align-items:center}
    .links a{color:var(--accent);text-decoration:none;font-weight:600}
    @media(max-width:880px){
      .grid{grid-template-columns:1fr; }
      .hero-gif{width:100%}
      .header{flex-direction:column;align-items:flex-start;gap:10px}
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="card">
      <div class="header">
        <div class="logo">SL</div>
        <div style="flex:1">
          <h1>Stress Level Classification Model</h1>
          <p class="lead">An AI tool that classifies student stress into <strong>Eustress</strong>, <strong>Distress</strong>, or <strong>No Stress</strong> using survey & lifestyle features. Ready for deployment (web & mobile).</p>
          <div class="badges">
            <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python" alt="python">
            <img src="https://img.shields.io/badge/TensorFlow-2.x-orange?style=for-the-badge&logo=tensorflow" alt="tensorflow">
            <img src="https://img.shields.io/badge/Keras-DL-red?style=for-the-badge&logo=keras" alt="keras">
            <img src="https://img.shields.io/badge/Scikit--Learn-ML-green?style=for-the-badge&logo=scikitlearn" alt="sklearn">
            <img src="https://img.shields.io/badge/Status-Showcase-success?style=for-the-badge" alt="status">
          </div>
        </div>

        <div style="display:flex;flex-direction:column;gap:8px;align-items:flex-end">
          <a class="btn" href="https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO" target="_blank">View on GitHub</a>
          <div class="small" style="text-align:right">Demo: Streamlit ready · Model: .h5 & .tflite</div>
        </div>
      </div>

      <!-- Hero animation -->
      <div class="gif-wrap" style="margin-top:18px">
        <img class="hero-gif" src="https://media.giphy.com/media/j5h8Hk5i0YwA0/giphy.gif" width="720" alt="hero gif">
        <div class="small">Interactive demo recommended: <a class="links" href="https://share.streamlit.io/YOUR_GITHUB_USERNAME/YOUR_REPO/app.py" target="_blank">Run Streamlit App</a></div>
      </div>

      <div class="grid" style="margin-top:22px">
        <div>
          <div class="box">
            <div class="section-title">📌 Project Overview</div>
            <p class="muted">This project uses survey features (emotional, physical, academic, social) to classify student stress. The notebook trains a TensorFlow/Keras model, evaluates performance, and exports a deployable .h5 model and a .tflite variant for mobile integration.</p>

            <div style="margin-top:14px">
              <div class="section-title">🧭 Quick Start</div>
              <pre><code># Clone
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO
cd YOUR_REPO

# Install
pip install -r requirements.txt

# Run notebook
jupyter notebook StressLevelModel.ipynb
              </code></pre>
            </div>

            <div style="margin-top:12px">
              <div class="section-title">📁 Project Structure</div>
              <div class="repo-structure">
<pre style="margin:0"><code>Stress-Classification-Model/
├─ StressLevelModel.ipynb
├─ StressLevelDataset.csv
├─ stress_model.h5
├─ stress_model.tflite (optional)
├─ requirements.txt
└─ README.md
</code></pre>
              </div>
            </div>

            <div style="margin-top:14px">
              <div class="section-title">📈 Results Snapshot</div>
              <div class="stats">
                <div class="stat"><strong>Accuracy</strong><div class="small">~89% (example)</div></div>
                <div class="stat"><strong>Classes</strong><div class="small">Eustress · Distress · No Stress</div></div>
                <div class="stat"><strong>Export</strong><div class="small">.h5 & .tflite</div></div>
              </div>
              <p class="small" style="margin-top:10px">Full metrics + confusion matrix included in notebook.</p>
            </div>

            <div style="margin-top:14px">
              <div class="section-title">🛠️ Tech Stack</div>
              <ul>
                <li>Python 3.10</li>
                <li>TensorFlow / Keras</li>
                <li>scikit-learn, pandas, numpy</li>
                <li>matplotlib, seaborn for visualization</li>
                <li>Streamlit for interactive demo (optional)</li>
              </ul>
            </div>
          </div>

          <div class="box" style="margin-top:18px">
            <div class="section-title">🔮 Future Improvements</div>
            <ul>
              <li>Deploy the Streamlit demo to Streamlit Cloud / HuggingFace Spaces</li>
              <li>Implement user questionnaire UI and logging</li>
              <li>Try tree-based baselines (XGBoost / RandomForest) & cross-validation</li>
              <li>Personalization & privacy-aware local model updating (on-device)</li>
            </ul>
          </div>
        </div>

        <aside>
          <div class="box">
            <div class="section-title">📥 Download / Links</div>
            <p class="small">Replace placeholder links below with your repo and demo URLs.</p>
            <div style="display:flex;flex-direction:column;gap:10px;margin-top:8px">
              <a class="btn" href="https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO/archive/refs/heads/main.zip" target="_blank">Download ZIP</a>
              <a style="text-decoration:none" href="https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO" target="_blank"><div class="box small" style="text-align:center">Open on GitHub</div></a>
              <a style="text-decoration:none" href="mailto:youremail@example.com"><div class="box small" style="text-align:center">Contact Author</div></a>
            </div>

            <div style="margin-top:12px">
              <div class="section-title">📷 Screenshots</div>
              <img src="https://media.giphy.com/media/xUOxf7p0W7xX1V5cU4/giphy.gif" alt="screenshot" style="width:100%;border-radius:8px;border:1px solid rgba(255,255,255,0.03)">
              <div class="small" style="margin-top:8px">Training history & confusion matrix are shown in the notebook.</div>
            </div>

            <div style="margin-top:12px">
              <div class="section-title">👨‍💻 Author</div>
              <p class="small">Antony — AI / ML enthusiast. <br>GitHub: <a class="links" href="https://github.com/YOUR_GITHUB_USERNAME" target="_blank">YOUR_GITHUB_USERNAME</a></p>
            </div>
          </div>

          <div class="box" style="margin-top:12px">
            <div class="section-title">📄 License</div>
            <p class="small">MIT License — include LICENSE file in repo if using this.</p>
            <div style="margin-top:8px">
              <div class="section-title">⚠️ Notes</div>
              <p class="small">Dataset is sourced from Kaggle. Do not expose personal or sensitive data. This demo is for educational and non-clinical use only.</p>
            </div>
          </div>
        </aside>
      </div>

      <div class="footer">
        <div style="display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap">
          <div>
            <strong>Want to run the demo?</strong> <span class="small">Install requirements & run the Jupyter notebook or the Streamlit app.</span>
          </div>
          <div style="text-align:right">
            <span class="small">Made with ❤️ • Antony</span><br>
            <span class="small">Star the repo if you found it useful ⭐</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
