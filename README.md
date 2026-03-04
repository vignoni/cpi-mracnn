# 🏆 Model Reference Adaptive Control with Neural Network Control

Welcome to the **Real-Time Control Systems Leaderboard**. This repository evaluates your MRAC NN control performance using **RMSE (Root Mean Square Error)** in Practice 2, Control PRedictivo e Inteligente - Universitat Politècnica de València.

The goal is to achieve the best tracking of the reference signal with your controller.

---

## 📊 Live Leaderboard & Plot
You can monitor the competition results and the latest submission plot here:
👉 **[[Competition Results]](https://vignoni.github.io/cpi-mracnn/)**

---

## 🚀 How to Participate

1. **Tune your controller:** Adjust your controler.
2. **Export your data:** Save your test results into a `.csv` file. 
   - **Important:** Your file must follow the standard export format (see below).
3. **Submit the Form:** Upload your file and enter your name in the official submission form:
   - 🔗 **[[GOOGLE FORM]](https://forms.gle/jV4DxNbFo26ZXHGg6)**

---

## 📋 CSV Data Format Requirements

To ensure the automated judge can read your results, your CSV file **must** have the following structure:

| Column | Data Description |
| :--- | :--- | 
| **A** | Row Index  |
| **B** | Timestamp |
| **C** | Reference |
| **D** | Output |

> [!CAUTION]
> **Do not change the order of the columns.** The evaluation script relies on these exact positions to calculate your score. 

### Example
| Index, | Time, | Ref, | Output |
| :--- | :--- | :--- | :--- |
| 0, | 0.397, |  1300, | 0    |  
| 1, | 0.417, |  1300, | 87   |  
| 2, | 0.437, |  1300, | 523  |  
| 3, | 0.457, |  1300, | 785  | 
|...|...|...|...|

---

## 📉 Evaluation Metric: RMSE

We use the **Root Mean Square Error** to rank your performance. 
- A **lower RMSE** means better tracking and higher precision.
- The **Grade** is automatically calculated based on your RMSE (Max: 10.00).

---

## 🛠️ Built With
- **Python**: Data processing and plotting (Pandas, Numpy, Matplotlib).
- **GitHub Actions**: Automated CI/CD pipeline for real-time assessment.
- **Google Forms & Apps Script**: Student submission bridge.
- **Tailwind CSS**: Live dashboard visualization.

**Good luck and may the best controller win!** 🤖🏎️
