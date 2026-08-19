# 🍽️ NutriGen — AI-Powered Personalized Nutrition

NutriGen is an **AI-powered nutrition assistant** that generates personalized meal plans and nutrition insights based on an individual's dietary preferences, allergies, health conditions, activity level, and fitness goals.

## ✨ Features

* 🥗 **Personalized Meal Planning** — Generate customized 7-day or day-specific meal plans.
* 🧬 **Nutrition Analysis** — Get AI-generated nutritional information for food items.
* ⚕️ **Health-Aware Recommendations** — Considers health conditions, allergies, and dietary restrictions.
* 🏃 **Activity-Based Planning** — Adapts recommendations according to activity level.
* 🍴 **Taste Preferences** — Allows users to specify preferred cuisines and foods.
* 🤖 **Generative AI** — Uses Google Gemini and OpenRouter-powered AI models.
* 🌐 **Web Interfaces & APIs** — Includes a Streamlit application and Flask API implementation.

## 🛠️ Tech Stack

| Technology               | Purpose                              |
| ------------------------ | ------------------------------------ |
| **Python**               | Core development                     |
| **Streamlit**            | Interactive meal-planning interface  |
| **Flask**                | REST API backend                     |
| **Google Gemini**        | Nutrition analysis & diet generation |
| **OpenRouter / Mistral** | AI-powered meal planning             |
| **Requests**             | API communication                    |

## 📁 Project Structure

```text
NutriGen/
│
├── app.py              # Streamlit AI meal planner
├── new.py              # Flask API for nutrition & diet plans
├── model.py            # Google Generative AI configuration
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

## ⚙️ How It Works

```text
User Preferences
      ↓
Dietary & Health Information
      ↓
AI Processing
      ↓
Personalized Nutrition / Meal Plan
      ↓
User-Friendly Output
```

The Streamlit application collects dietary restrictions, allergies, health conditions, activity level, taste preferences, and the selected day, then sends the information to an AI model to generate a personalized meal plan.

The Flask implementation provides API endpoints for:

* `/nutrition` — Get nutritional information for a food item
* `/diet_plan` — Generate a personalized diet plan

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/techy-ops/NutriGen.git
cd NutriGen
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Keys

Store your AI API keys securely using environment variables instead of hard-coding them in source files.

Example:

```env
GOOGLE_API_KEY=your_google_api_key
OPENROUTER_API_KEY=your_openrouter_api_key
```

### 5. Run the Streamlit application

```bash
streamlit run app.py
```

The application will open in your browser.

## 🔌 API Endpoints

### Nutrition Information

**POST** `/nutrition`

```json
{
  "food_item": "Oatmeal"
}
```

### Personalized Diet Plan

**POST** `/diet_plan`

```json
{
  "age": 22,
  "weight": 65,
  "height": 170,
  "activity_level": "Moderately active",
  "goal": "Weight maintenance"
}
```

## 🎯 Use Cases

* Personalized meal planning
* Basic nutrition exploration
* Fitness-oriented diet planning
* Dietary restriction management
* AI-assisted food recommendations

## 🔮 Future Enhancements

* 📊 Calorie and macro tracking
* 👤 User profiles and meal history
* 🛒 Automated grocery lists
* 📱 Mobile application
* 🥘 Regional and culturally personalized recipes
* 📈 Nutrition dashboards and progress tracking
* 🔐 Secure authentication and database integration

## ⚠️ Disclaimer

NutriGen provides **AI-generated nutritional information and meal suggestions for educational purposes**. It is not a substitute for professional medical or dietary advice. Users with medical conditions should consult a qualified healthcare professional.

ou find NutriGen useful, consider giving the repository a star!
