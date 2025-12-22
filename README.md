# 🧠 Custom Quiz Creator Web App

A simple, flexible, and user-friendly web application that allows users to **create and attempt custom quizzes** using JSON files or predefined quiz data.  
Users can set their own **test duration**, upload quiz data, and get **instant results with explanations**.

---

## 🚀 Features

- 📂 Upload quiz using a **JSON file**
- ✍️ Create quiz using **custom JSON format**
- ⏱️ Set **custom time duration** for the test
- ▶️ Start quiz with a **live countdown timer**
- ⏹️ Automatic submission when time is over
- ✅ Manual quiz submission option
- 📊 Result summary with:
  - Total marks
  - Correct answers highlighted
  - User answers vs correct answers
  - Explanation for each question

---

## 🖥️ How the Website Works

When you open the website, you will see **two main options**:

### 1️⃣ Upload JSON File
- You can upload a quiz JSON file directly.
- Multiple ready-made quiz JSON files are available on GitHub.

🔗 **Sample JSON Files Repository for Salesforce AgentForce Certification Practice**  
👉 https://github.com/cksite/quize_app/tree/main/AgentForce%20Test%20Json%20File

You can:
- Download any JSON file from this repository
- Upload it on the website
- Start your quiz instantly

---

### 2️⃣ Input Time Duration
- Enter the quiz duration (in seconds)
- The timer starts as soon as the quiz begins
- When time is over:
  - Quiz is **automatically submitted**
  - OR you can submit manually using the **Submit Quiz** button

---

## 📝 Quiz Flow

1. Upload JSON file **OR** create your own quiz JSON
2. Enter test duration
3. Click **Start Custom Quiz**
4. Attempt questions while the timer runs
5. Quiz auto-submits when time ends (or manual submit)
6. Result page shows:
   - Total score (at the top)
   - Correct answers highlighted
   - Your answer vs correct answer
   - Explanation for every question

---

## 📌 JSON File Format (IMPORTANT)

If you want to create your **own quiz**, your JSON file **must follow this format exactly** 👇

```json
{
  "time_limit": 1800,
  "questions": [
    {
      "question": "Of the following, which is the closest approximation of (50.2*0.49)/199.8?",
      "options": ["0.100", "0.115", "0.125", "0.150"],
      "correct_index": 2,
      "explanation": "Approximating (50.2×0.49)/199.8 as 50×0.5/200 gives 25/200 = 0.125."
    },
    {
      "question": "How many prime numbers between 1 and 100 are factors of 7150?",
      "options": ["2", "3", "4", "5"],
      "correct_index": 2,
      "explanation": "7150 = 2 × 5² × 11 × 13, so there are 4 distinct prime numbers."
    }
  ]
}
