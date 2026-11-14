<<<<<<< HEAD
# AgriVision – Smart Crop Recommendation System

AgriVision is an IoT-enabled smart agriculture project that combines soil monitoring, machine learning-based crop recommendation, and market-price analysis in a web dashboard.

## Project contents

- `index.html` – web dashboard interface
- `style.css` – dashboard styling
- `server.py` – Python HTTP backend
- `Crop.csv` – crop recommendation dataset
- `crop_model.pkl` – trained crop recommendation model
- `market_price_model.pkl` – trained market-price model
- `market_price_features.pkl` – feature information used by the market model
- `images/` – dashboard image assets

## Requirements

- Python 3
- pandas
- joblib
- scikit-learn
- `curl` available on your system for the market-data request

Install the Python packages:

```bash
pip install -r requirements.txt
```

## Configure the Data.gov.in API key

For security, the API key is not stored in this repository. Set your own valid Data.gov.in API key as an environment variable before starting the server.

**Windows PowerShell:**

```powershell
$env:DATA_GOV_API_KEY="YOUR_API_KEY"
python server.py
```

**macOS / Linux:**

```bash
export DATA_GOV_API_KEY="YOUR_API_KEY"
python server.py
```

Then open `http://localhost:8000` in your browser.

If the market-price feature is used, a valid API key and internet connection may be required. The dashboard also loads Chart.js from a CDN, so its charts may require internet access.

## Important notes

- The trained `.pkl` models are included. They may require compatible versions of scikit-learn and related Python libraries.
- Use your own sensor hardware and configuration to send live soil readings to the backend.
- Dataset and model outputs should be validated before using them for real farming decisions.
=======
# AgriVision
>>>>>>> ff5579d94d4e340c3dffe4f56ef86e2924df4ac7
