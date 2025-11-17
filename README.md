# NutriTrack – Gamified Nutrition Learning App 🥝⚽  
*A playful web app that teaches young athletes how to eat smart before, during, and after a match.*

---

## 🌟 Overview  

NutriTrack turns nutrition into a game:  
Kids build a **food lineup**, fight **Food Bosses**, and learn with a friendly animated **Kiwi Coach**.

This is a PROTOTYPE originally created for a hackathon

---

## 🎮 Core Features  

### 🥝 Kiwi Coach (Interactive Assistant)  
- Floating animated Kiwi coach  
- Gives simple nutrition tips  
- Answers predefined questions  
- Can read answers out loud (speech synthesis)  
- Cute dialog bubble + dedicated answer screen  

---

### 🥦 Food List + Barcode Search Mode in Open Food Fact data base 
- Browse a list of foods with:
  - **NutriScore**
  - **EcoScore**
- In the future: implement a barcode scan with a camera
- Add any food to your lineup
- Help creating improving OpenFoodFact DataBase by submitting a product

---

### ⚽ Match & Meal Strategy Builder  

Organize foods into match phases:

- ⚡ **Pre-match** (slow energy)
- 🔥 **Mid-match** (quick fuel)
- 💧 **Post-match** (recovery)

NutriTrack computes:

- 🩺 Health Score  
- 🌍 Eco Score  
- 🏆 Final Performance Score  

Then suggests a simple recipe based on the main food.

---

### 👑 Food Boss Battles  

Turn good nutrition into a challenge:

- **Win** → 🎉 victory popup with confetti + happy Kiwi  
- **Lose** → 😢 defeat popup with sad Kiwi + motivational message  

Everything stays playful and positive.

---

### ➕ Add New Products  

From the **New Product** screen, users can add:

- Product name  
- Brand  
- Barcode  
- NutriScore  
- EcoScore  

The new food appears immediately in the list and can be used in lineups.

---

## 🛠 Tech Stack  

### Frontend
- HTML  
- Tailwind CSS  
- Vanilla JavaScript  
- Custom animations, floating coach, modals, confetti  

### Backend
- Python  
- FastAPI  
- Uvicorn (dev server with reload)  
- Simple in-memory or file-based “database” of products  

---

## 📦 Installation  

```bash
git clone https://github.com/YanisLaribi/NutriTrack.git
cd NutriTrack/backend

python -m venv venv
venv\Scripts\activate

python3 -m venv venv
source venv/bin/activate

pip install -r requirements.txt

uvicorn main:app --reload

Open in your browser:
👉 http://127.0.0.1:8000
```

