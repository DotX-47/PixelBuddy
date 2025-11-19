# 🎮 PixelBuddy — Steam PC Compatibility Checker

PixelBuddy is a modern and intuitive Streamlit-based application designed to help gamers quickly determine if their PC can run any Steam game.  
By automatically analyzing your system’s hardware and comparing it with Steam’s official system requirements, PixelBuddy provides performance estimates, graphics recommendations, and compatibility warnings.

---

![PixelBuddy Logo](PixelBuddy/logp.svg)

---

## 🌟 Why PixelBuddy?

Most PC gamers often struggle with questions like:
- *“Can my PC run this game?”*  
- *“What graphics settings will I get?”*  
- *“Do I meet the recommended specs?”*

PixelBuddy answers all of these instantly—no guesswork, no searching through specs, and no confusion.

---

![PixelBuddy Screenshot](./ss.png)

---

## 🚀 Features

### 🖥 Automatic Hardware Detection
PixelBuddy scans your system and collects:
- CPU model & architecture  
- GPU model & VRAM  
- Installed RAM  
- Total disk space  
- Operating system  

### 🔍 Steam Game Search
- Search any Steam game by name  
- Displays top matching results with names & App IDs  

### 📥 Steam Requirement Fetching  
PixelBuddy retrieves requirements directly from Steam’s API, including:
- Minimum Requirements  
- Recommended Requirements  

These include OS, CPU, Graphics card, VRAM, RAM, Storage, and other notes.

### 🧠 Smart System Comparison
The app compares your specs with the game's requirements using:
- Custom CPU scoring  
- GPU performance scoring  
- VRAM & RAM evaluation  
- Overall rating from 0–100  

### 🎯 Performance Prediction
PixelBuddy provides:
- Can-Run Indicator (Yes/No)  
- Graphics Level Estimate (Low → High/Ultra)  
- Estimated FPS  
- Warnings about weak components  

### 🧾 Requirements Table
It also displays a clean system requirement table extracted from Steam.

---

![PixelBuddy Screenshot](PixelBuddy/ss1.png)

---

## 🛠 Technologies Used

- **Streamlit** – UI Framework  
- **Python** – Core Logic  
- **psutil** – Hardware detection  
- **GPUtil** – GPU scanning  
- **BeautifulSoup4** – Parsing Steam HTML  
- **Requests** – Steam API calls  
- **Regex** – Requirement extraction and matching  

---

## 📦 Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/DotX-47/PixelBuddy.git
cd PixelBuddy
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the App
```bash
streamlit run app.py
```

---

## 🧩 How It Works (Detailed)

1. The app analyzes your hardware using:
   - platform  
   - psutil  
   - GPUtil  

2. You type a game name into the search bar.

3. PixelBuddy fetches the game list from Steam.

4. After selecting a game, PixelBuddy:
   - Downloads Steam PC requirements  
   - Parses HTML for min/recommended specs  
   - Extracts CPU, GPU, RAM, and storage info  

5. Your system specs are compared using:
   - Scoring algorithms  
   - Hardware ratios  
   - Performance thresholds  

6. PixelBuddy outputs:
   - Can-run status  
   - Graphics level  
   - Estimated FPS  
   - A detailed notes section  

---

## 🤝 Contributing

You’re welcome to contribute!  
Whether it’s bug fixes, feature suggestions, or UI improvements — feel free to submit a pull request.



---

## ⭐ Show Your Support

If you find PixelBuddy useful, please ⭐ star the repository!  
Your support motivates further development.  
  
