# 📊 LeetMetrics

> **Turn your LeetCode profile into meaningful metrics.**

LeetMetrics is a lightweight web application that lets you enter a **LeetCode username** and instantly view important problem-solving statistics in a clean and focused interface.

Instead of repeatedly checking different parts of your LeetCode profile, LeetMetrics brings the useful information together in one place.

---

## ✨ What is LeetMetrics?

LeetMetrics is built around a simple idea:

**Enter a username → Fetch the data → Understand your progress.**

The application communicates with the **LeetCode GraphQL API** to retrieve user-related problem-solving data and transforms that information into readable metrics.

It was built with a focus on:

- 🎯 Simplicity
- ⚡ Fast interaction
- 📊 Data visualization
- 🧩 Clean UI
- 🛠️ Practical JavaScript implementation

---

## 🚀 Features

### 👤 LeetCode Profile Search
Enter any valid LeetCode username and search for the corresponding profile data.

### 📊 Problem Statistics
View problem-solving statistics across different difficulty levels:

- 🟢 Easy
- 🟡 Medium
- 🔴 Hard
- 📚 Total Questions

### 📈 Submission Metrics
Get useful information about the user's submission activity and progress.

### 🔎 Username Validation
The application handles invalid or unavailable usernames instead of silently displaying incorrect information.

### ⚡ Dynamic Data
Statistics are fetched when the user searches rather than relying on hardcoded values.

### 🎨 Clean Interface
A minimal interface keeps the focus on the data instead of unnecessary visual clutter.

### ❌ Error Handling
Network/API failures are handled gracefully and communicated to the user.

---

## 🧠 How It Works

The application follows a simple data flow:

```text
              ┌─────────────────┐
              │  Enter Username │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │  Search Button  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ GraphQL Request │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │  LeetCode Data  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Process Response │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Display Metrics │
              └─────────────────┘
