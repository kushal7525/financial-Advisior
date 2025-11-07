
# AI Financial Coach Agent  
*A multi-agent personal finance coach powered by Google’s ADK and modern LLMs*

## 📘 Overview  
The **AI Financial Coach Agent** is an intelligent, modular system designed to evaluate personal financial data and provide actionable budgeting, saving, and debt-management insights.  
Built using Google’s **Agent Development Kit (ADK)**, it leverages a coordinated multi-agent workflow to deliver comprehensive, user-friendly financial recommendations.

This project is a great starting point for:
- Developers learning agentic architectures
- AI researchers building financial-domain assistants
- Individuals aiming to understand and improve their finances

---

## ✅ Key Features
✅ Multi-agent workflow (budgeting → savings → debt strategy)  
✅ CSV + manual expense entry  
✅ Automated spending categorisation  
✅ Smart insights & improvement suggestions  
✅ Visualizations: Pie/Bar/Line charts for clear understanding  
✅ Flexible and extensible architecture  
✅ User-friendly Streamlit interface  

---

## 🧩 Multi-Agent System  
The system consists of specialized agents working sequentially:

| Agent | Function |
|-------|----------|
| **Budget Analysis Agent** | Reviews income & expenses, highlights waste & patterns |
| **Savings Strategy Agent** | Generates personalized savings recommendations |
| **Debt Reduction Agent** | Suggests payoff strategies to minimize debt faster |

The agents share state, allowing each to build on the previous step’s output.

---

## ⚙️ Technology Stack
| Component | Purpose |
|----------|---------|
| **Python 3.10+** | Development runtime |
| **Google ADK** | Multi-agent orchestration |
| **Gemini API** | LLM-powered financial analysis |
| **Streamlit** | UI + data visualization |
| **Pandas / Matplotlib** | Data parsing + graphing |

---

## 🚀 Getting Started

### ✅ Prerequisites
- Python 3.10+
- Google Gemini API Key (via Google AI Studio)

---

### 🔧 Installation

```bash
git clone https://github.com/kushal7525/financial-Advisior.git
cd financial-Advisior

python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

pip install -r requirements.txt
````

Create a `.env` file:

```
GOOGLE_API_KEY=your_gemini_api_key
```

---

## ▶️ Run the App

```bash
streamlit run financial-Advisior.py
```

Then open the URL displayed in your terminal (e.g. `http://localhost:8501`).

---

## 📁 CSV Format

Upload a CSV file containing expense data:

| Column     | Description        |
| ---------- | ------------------ |
| `Date`     | Format: YYYY-MM-DD |
| `Category` | Spending category  |
| `Amount`   | Numeric value      |

Example:

```
Date,Category,Amount
2024-01-01,Food,150.50
2024-01-05,Transportation,45.00
2024-01-10,Housing,1200.00
```

You may also enter expenses manually through the UI.

---

## 🔍 How It Works

1. **User submits financial data** (CSV or manual)
2. **Agents collaborate in sequence** using ADK:

   * Budget → Savings → Debt
3. Each agent receives the current state and contributes new insights
4. Recommendations + visualization are displayed to the user

Flow Diagram (Conceptual):

```
[User Input] → Budget Agent → Savings Agent → Debt Agent → Visual Output
```

---

## 📈 Visualizations

The system generates intuitive charts including:

* Spending distribution (Pie)
* Monthly income vs expenses (Bar / Line)
* Debt payoff projections

These insights allow users to immediately pinpoint problem areas and opportunities.

---

## 🔮 Extending the System

This architecture is modular—adding new agents is easy.

Ideas:

* ✅ Investment Planning Agent
* ✅ Tax Estimation Agent
* ✅ Goal-based agent (Car, Travel, Wedding planning)
* ✅ Financial-education suggestions
* ✅ Data persistence layer (DB)

---

## 🛡 Disclaimer

This project is intended for **educational purposes only**.
It does **not** provide certified financial advice.
Consult a licensed financial professional before making real decisions.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Open a pull request


## ⭐ Acknowledgments

* Google AI & Gemini
* Python open-source ecosystem

---



