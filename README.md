# 🌍 Capital City Quiz

A fun web quiz where users guess the **capital city of a randomly selected country**.

Built using **Node.js, Express, PostgreSQL, and EJS**.
If the answer is correct ✅ the score increases.
If the answer is wrong ❌ the game ends.

---

## ✨ Features

🌎 Random country questions

🧠 Test knowledge of world capitals

📊 Live score tracking

✔ Instant answer feedback

❌ Game ends on wrong answer

---

## 📸 Screenshots

(Add your screenshots here)

<img width="1919" height="1053" alt="image" src="https://github.com/user-attachments/assets/5b844546-9880-48ba-937a-d5a307cd50e5" />

---

## 🛠 Tech Stack

**Backend**

* Node.js
* Express.js

**Frontend**

* EJS
* HTML
* CSS

**Database**

* PostgreSQL

---

## 📁 Project Structure

```
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
```

---

## 🗄 Database Setup

Create database

```
CREATE DATABASE world;
```

Create table

```
CREATE TABLE capitals (
  id SERIAL PRIMARY KEY,
  country VARCHAR(100),
  capital VARCHAR(100)
);
```

Import the data from **capitals.csv**.

---

## ⚙ Database Configuration

Replace the database credentials in `index.js`.

```
const db = new pg.Client({
  user: "username",
  host: "localhost",
  database: "world",
  password: "password",
  port: port_number
});
```

Example:

```
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

```
git clone https://github.com/yourusername/capital-city-quiz.git
```

Go to the project folder

```
cd capital-city-quiz
```

Install dependencies

```
npm install
```

---

## ▶ Run the Application

```
node index.js
```

Open in browser

```
http://localhost:3000
```

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
