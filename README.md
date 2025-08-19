# Zelta Labs PS

## 📌 Overview
I am Akshat Rai, a sophomore at IIT(ISM) Dhanbad, pursuing B.Tech in Engineering Physics.  

I am targeting InterIIT Tech Meet 14.0. This problem statement by Zelta Labs came in 12.0 and 13.0 editions. In 11.0, this was given by QuantInsti, however we had to build Price Action strategies (which I'll try to build here) and do stuff on Indian Stock Market.  

Data is in a ZIP file as it is huge (544 MB), extract the ZIP file and make sure the `data/` folder is in the root repo.

---

## ⚙️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/AkshatRai07/ZeltaLabsPSPrep.git
cd ZeltaLabsPSPrep
```

### 2. Create a virtual environment
```bash
python -m venv venv
```

### 3. Activate the environment
- **Linux / MacOS**
  ```bash
  source venv/bin/activate
  ```
- **Windows (PowerShell)**
  ```bash
  .\venv\Scripts\activate
  ```

### 4. Install dependencies
```bash
pip install -r requirements.txt
```

### 5. Add venv to Jupyter
```bash
python -m ipykernel install --user --name=venv --display-name "Python (venv)"
```

---

## ▶️ Usage

1. Start Jupyter Notebook
   ```bash
   jupyter notebook
   ```
2. Open `SnR.ipynb`
3. Make sure the kernel is set to **Python (venv)**  
   (**Kernel → Change Kernel → Python (venv)**)

---

## 📂 Project Structure
```
.
├── data/
│   ├── btcData/        # Bitcoin-related datasets
│   ├── ethData/        # Ethereum-related datasets
│
├── SnR.ipynb           # Main analysis notebook
├── requirements.txt    # Python dependencies
├── .gitattributes      # Git LFS configuration
├── .gitignore          # Ignored files/folders
├── data.zip            # Example dataset archive (tracked via LFS)
└── README.md           # Project documentation
```

---
## 📦 Git LFS (Large File Storage)

This project uses **Git LFS** to handle large files (datasets, `.zip`, `.csv`, etc.).  

### Install Git LFS
```bash
# Linux / MacOS
brew install git-lfs   # (Mac with Homebrew)
sudo apt-get install git-lfs   # (Ubuntu/Debian)

# Windows (Chocolatey)
choco install git-lfs
```

### Initialize Git LFS
```bash
git lfs install
```

### Pull Large Files
After cloning the repo, run:
```bash
git lfs pull
```

This ensures all large dataset files (like `data.zip`) are downloaded properly.

---

## 🛠️ Development Notes
- Always create a new branch for new features or experiments.
- Keep `requirements.txt` updated after installing new packages:
  ```bash
  pip freeze > requirements.txt
  ```
- Do **not** commit the `venv/` and `data/` folders (already in `.gitignore`).