# 🌋 Earthquake Pattern Discovery

Spatiotemporal clustering app to identify seismic zones, aftershock clusters, and high-risk regions from USGS earthquake data.

## 🚀 Deploy to Streamlit Cloud

### Step 1 — Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### Step 2 — Deploy on Streamlit Cloud
1. Go to [share.streamlit.io](https://share.streamlit.io)
2. Click **"New app"**
3. Select your GitHub repo
4. Set **Main file path** → `app.py`
5. Click **Deploy!**

## 📁 Required File Structure
```
your-repo/
├── app.py              ← main Streamlit app
├── query.csv           ← earthquake dataset
├── requirements.txt    ← Python dependencies
└── .streamlit/
    └── config.toml     ← theme & server config
```

> ⚠️ **Important:** `query.csv` must be committed to the repo alongside `app.py`.

## 📦 Dependencies
See `requirements.txt` — no Mapbox token required, all map styles are free.

## 🖥️ Run Locally
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Features
- 🗺️ Interactive global seismic map (cluster / magnitude / depth coloring)
- 📡 DBSCAN & K-Means clustering with tunable parameters
- ⚠️ Risk zone scoring and heatmap
- 📈 Temporal patterns, hourly distribution, aftershock detection
- 🔬 PCA, 3D scatter, Gutenberg-Richter, correlation matrix
