# 🛒 AI Merch Maker Lite

An automated backend pipeline that generates AI-powered product listings, creates product mockups, and publishes them to Shopify — built as part of an internship assignment.

---

## 📌 Overview

**AI Merch Maker Lite** simulates a mini eCommerce automation workflow by:

1. **Generating product titles, descriptions, and tags** using AI.
2. Creating or simulating **product images**.
3. Producing **mockup images** using a JavaScript (Node.js) mockup server.
4. Publishing products to **Shopify** via the Admin API (with a PHP fallback for simulation).

---

## 🛠 Tech Stack

- **Python** → AI text generation, automation, Shopify API integration
- **JavaScript (Node.js)** → Mockup generation server
- **PHP** → Fake product publisher fallback
- **Shopify API** → Real store integration

---

## 📂 Project Structure

```
AI-Merch-Maker/
│── orchestrator.py          # Main pipeline runner
│── text_generator.py        # AI-based product title/description/tags generator
│── shopify_uploader.py      # Shopify API integration
│── publish.php              # Fake product publisher (PHP fallback)
│── mockup-generator/        # Node.js mockup server
│   └── server.js
│── templates/               # Mockup templates (if any)
│── requirements.txt         # Python dependencies
│── package.json             # Node.js dependencies
│── .env.example             # Example environment variables
│── README.md                # This file
```

---

## ⚙️ Setup & Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/YOUR-USERNAME/ai-merch-maker-lite.git
cd ai-merch-maker-lite
```

### 2️⃣ Install Python Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Install Node.js Dependencies
```bash
cd mockup-generator
npm install
cd ..
```

### 4️⃣ Create `.env` File
Create a `.env` file in the project root with the following values:
```env
OPENROUTER_API_KEY=your_api_key_here
SHOPIFY_STORE_URL=your_store.myshopify.com
SHOPIFY_ADMIN_API_KEY=your_admin_api_key
SHOPIFY_ADMIN_PASSWORD=your_admin_password
```

---

## 🚀 Running the Project

### Step 1 – Start the Mockup Server
```bash
cd mockup-generator
node server.js
```

### Step 2 – Run the Orchestrator
```bash
python orchestrator.py
```

---

## 📸 Expected Output

**Console Logs Showing:**
- AI-generated product title, description, and tags
- Mockup image creation
- Shopify product upload confirmation

**File Output:**
```
mockup.png saved in the root folder
```

**Shopify Output:**
- Product visible in Shopify Admin → Products

---

## 📜 License
This project is for **educational and internship evaluation purposes only**.
