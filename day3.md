# 📅 Day 3 – Log Analyzer Project

---

## 🎯 Goal

Analyze log files, extract errors, and organize results.

---

## 📁 Project Structure

day3/
├── logs/
├── results/
└── backup/

---

## 📄 Log Files

* app.log
* server.log
* system.log

Each file contains:

* info
* warning
* error

---

## 🔍 Step 1 – Find all errors

grep error logs/*.log

* finds all lines containing "error"

---

## 🔢 Step 2 – Sort errors

grep error logs/*.log | sort

* sorts all error lines

---

## 🔽 Step 3 – Get last 2 errors

grep error logs/*.log | sort | tail -n 2

* shows last 2 lines

---

## 💾 Step 4 – Save results

grep error logs/*.log > results/error.txt

* saves all error lines into a file

---

## 🔄 Step 5 – Backup logs

rsync -a logs/ backup/

* creates backup of log files

---

## 🧠 Key Concepts Used

* grep → filtering
* sort → sorting
* pipe (|) → chaining commands
* tail → selecting output
* redirection (>) → saving output
* rsync → backup

---

## ⚠️ Notes

* commands depend on current directory
* always check path with pwd
* use relative paths correctly

---
