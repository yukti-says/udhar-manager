# 💸 Udhar Manager

A simple web application to manage and record customer credit ("Udhar") transactions. Built using **HTML**, **CSS**, **JavaScript**, and **Firebase Firestore** for real-time cloud storage.

---

## 📌 Features

- 📥 Add customer transaction entries via a form.
- 🧮 Automatically calculate and display balance (`Total - Paid`).
- 📅 Auto-generate and save timestamp of each entry.
- 📋 View all customer records in a responsive table.
- ☁️ Real-time data handling using **Firebase Firestore**.

---

## 🛠️ Tech Stack

| Tech               | Purpose                                 |
|--------------------|------------------------------------------|
| HTML               | Webpage structure                        |
| CSS                | Styling & layout (`style.css`)           |
| JavaScript         | Dynamic behavior & Firebase integration  |
| Firebase Firestore | Cloud-based NoSQL database               |

---

## 🔧 Project Structure
Udhar System/
├── index.html # Main app file (HTML + JS + Firebase logic)
├── style.css # Styling for the app

Firebase SDK methods used:

```initializeApp()`` – Initializes Firebase app

```getFirestore()``` – Initializes Firestore DB

```addDoc()``` – Add a new document (record)

```getDocs()`` – Fetch all documents

## 🧮 How It Works
# 1. Form Submission

Takes user input: Customer Name, Total Amount, Amount Given
Calculates Balance = Total - Paid
Stores the data along with timestamp into Firestore
Resets the form and reloads the table

# 2. Record Table
Fetched from Firestore on load and after every entry

# Shows:

Customer Name
Total Amount
Paid Amount
Remaining Balance
Timestamp (Date & Time)

## ✅ Validations
Required fields: Name, Total, Given
All inputs are trimmed and validated
Prevents empty or invalid data
Clears form after successful entry

## 📊 Example Output
Name	Total (₹)	Paid (₹)	Balance (₹)	Date & Time
Ramesh	₹5000	₹3000	₹2000	25/05/2025, 10:45 AM

## 🚀 Getting Started

# 1. Clone the Repo

```bash ```
git clone https://github.com/yukti-says/udhar-manager.git
cd udhar-manager

# 2. Setup Firebase

Go to Firebase Console
Create a project
Enable Firestore in Build → Firestore Database
Replace the Firebase config in your index.html

# 3. Run the App

Just open ```index.html`` in any modern browser.

## 🌐 Firebase Hosting (Optional)

You can deploy your app using Firebase Hosting:

```bash
Copy code
npm install -g firebase-tools
firebase login
firebase init```

# Choose "Hosting", set public directory to "."

firebase deploy
🧠 Future Enhancements
🔍 Search/filter by customer name
✏️ Edit/delete entries
📱 Fully responsive mobile UI
🔐 Add user login with Firebase Auth
📤 Export records as CSV/PDF
📊 Visual analytics with charts

## 👩‍💻 Author

# Yukti Sahu

🎓 MCA Student | 💻 Aspiring Full-Stack Developer


## 📁 License

This project is open-source and free to use for personal and educational purposes.