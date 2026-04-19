# 🌍 Capital City Quiz

A fun web quiz where users guess the **capital city of a randomly selected country**.

Built using **Node.js, Express, PostgreSQL, and EJS**, this project tests your knowledge of world capitals.
If your answer is correct ✅ your score increases. If it's wrong ❌ the game ends!

---

## ✨ Features

🌎 Random country questions
🧠 Test your knowledge of world capitals
📊 Live score tracking
✔ Instant answer feedback
❌ Game ends on wrong answer
⚡ Fast Express server
🗄 Data stored in PostgreSQL

---

## 📸 Screenshots

<img width="1919" height="1060" alt="image" src="https://github.com/user-attachments/assets/9a0e5250-783e-4940-8995-85a9f67ee519" />

---

## 🛠 Tech Stack

**Backend**
🟢 Node.js
🚀 Express.js

**Frontend**
🎨 EJS
📄 HTML
💅 CSS

**Database**
🐘 PostgreSQL

---

## 📁 Project Structure

capital-city-quiz
│
├── public
│   └── styles
│       └── main.css
│
├── views
│   └── index.ejs
│
├── capitals.csv
├── index.js
├── package.json
└── package-lock.json

---

## 🗄 Database Setup

Create database

CREATE DATABASE world;

Create table

CREATE TABLE capitals (
id SERIAL PRIMARY KEY,
country VARCHAR(100),
capital VARCHAR(100)
);

Import the data from **capitals.csv** into the table.

---

## ⚙ Database Configuration

Before running the project, update the database credentials inside **index.js**.

Replace the placeholders with your PostgreSQL details:

```javascript
const db = new pg.Client({
  user: "username",
  host: "localhost",
  database: "world",
  password: "password",
  port: port_number
});
```

Example configuration:

```javascript
const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "world",
  password: "your_password",
  port: 5432
});
```

---

## 💻 Installation

Clone the repository

git clone https://github.com/yourusername/capital-city-quiz.git

Go to the project folder

cd capital-city-quiz

Install dependencies

npm install

---

## ▶ Run the Application

node index.js

Open in your browser

http://localhost:3000

---

## 🎮 How the Quiz Works

1️⃣ The server loads countries and capitals from PostgreSQL.
2️⃣ A random country is selected.
3️⃣ The user enters the capital city.
4️⃣ Correct answer → score increases 📈
5️⃣ Wrong answer → game over ❌

---

## 🚀 Future Improvements

⏳ Add timer for questions
🏆 Add leaderboard
🏳 Show country flags
📊 Store high scores
🎯 Add difficulty levels

---

✨ *A simple and fun way to practice world capitals!* 🌎
