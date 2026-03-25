

# 📊 COAL Grade Predictor (MASM + Irvine32)

## 📌 Overview

This project is a **COAL (Computer Organization & Assembly Language) Grade Predictor** written in **x86 Assembly (MASM)** using the **Irvine32 library**.

It predicts a student’s **final exam performance** and **overall grade** based on:

* Midterm scores
* Quiz marks
* Assignment marks

The program uses **linear regression**, along with **mean and standard deviation**, calculated from historical student data.

---

## ⚙️ Features

* ✅ User input with validation
* ✅ Mean calculation of datasets
* ✅ Standard deviation calculation
* ✅ Linear regression implementation
* ✅ Final weightage prediction
* ✅ Automatic grade calculation (A+ → F)


## 🧠 Concepts Used

* Assembly Language (MASM)
* Irvine32 Library
* Arrays and loops
* Procedures (PROC)
* Mathematical modeling:

  * Mean
  * Standard deviation
  * Linear regression

---

## 📂 Data Used

Two datasets are used:

* `student_overall` → Overall marks out of 50
* `student_final` → Final exam marks

These datasets are used to train the regression model.

---

## 🛠️ Requirements

To run this project, you need:

* MASM (Microsoft Macro Assembler)
* Irvine32 Library (`Irvine32.inc`, `Irvine32.lib`)
* Windows OS
* Visual Studio / VS Code (recommended)

---

## ▶️ How to Run

1. Install MASM and Irvine32 library

2. Place files:

   * `Irvine32.inc`
   * `Irvine32.lib`

3. Assemble and run using:

```bash
ml /c /coff filename.asm
link /subsystem:console filename.obj Irvine32.lib
```

---

## 🧾 Program Flow

1. Display welcome message

2. Take input:

   * Mid1 (out of 15)
   * Mid2 (out of 15)
   * Quiz (out of 10)
   * Assignment (out of 10)

3. Validate input ranges

4. Compute:

   * Mean
   * Standard deviation
   * Regression coefficients

5. Predict:

   * Final exam marks
   * Total marks out of 100

6. Display grade:

```
A+, A, A-, B+, B, B-, C+, C, C-, D+, D, F
```

---

## 📈 Grade Criteria

| Marks | Grade |
| ----- | ----- |
| 90+   | A+    |
| 86+   | A     |
| 82+   | A-    |
| 78+   | B+    |
| 74+   | B     |
| 70+   | B-    |
| 66+   | C+    |
| 62+   | C     |
| 58+   | C-    |
| 54+   | D+    |
| 50+   | D     |
| <50   | F     |

---

## ⚠️ Notes

* Input must follow given ranges:

  * Mid terms ≤ 15
  * Quiz ≤ 10
  * Assignment ≤ 10
* Invalid input will be re-requested
* Uses integer arithmetic (approximation)

---

## 👨‍💻 Author

* M. Hammas Alauddin 
* M.Sarim Khurram
* Ali Raza

---

## 🚀 Future Improvements

* Floating-point precision
* GUI version
* File-based dataset input
* Graph visualization

--
