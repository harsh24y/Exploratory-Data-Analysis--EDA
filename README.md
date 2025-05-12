# 📊 Exploratory Data Analysis (EDA) – Gender & Age Group Insights

This project focuses on performing **Exploratory Data Analysis (EDA)** on employee demographic data to uncover patterns related to **gender distribution** and **age group categorization** using Python libraries such as **pandas**, **matplotlib**, and **seaborn**.

---

## 📸 Screenshot
![Screenshot 2025-05-12 223616](https://github.com/user-attachments/assets/65e1e307-ee5e-4cb5-ba55-3c05c02a7edf)
![Screenshot 2025-05-12 223631](https://github.com/user-attachments/assets/970897ca-9cc8-4cc5-97a9-dd39a76ea367)

![Screenshot 2025-05-12 223648](https://github.com/user-attachments/assets/3f384be7-eef8-4e6e-8167-67e674c55e59)
![Screenshot 2025-05-12 223707](https://github.com/user-attachments/assets/26c6356c-5a8a-4079-b095-dd08a808f17b)

---

## 🧠 Problem Statement

A company provided a dataset of its employees with attributes such as **gender** and **age**. The goal was to:
- Count how many male and female employees are working.
- Categorize employees into relevant **age groups** for workforce analysis.

---

## 🛠️ Tools & Technologies

| Technology | Purpose |
|------------|---------|
| Python     | Data analysis and visualization |
| Pandas     | Data manipulation |
| Seaborn    | Visualization |
| Matplotlib | Plotting graphs |
| IBM SkillsBuild | Internship learning platform |
| IBM Watson / IBM Cloud | Exposure to AI & cloud integration (supporting tools) |

---

## 🚀 Steps Followed

1. **Data Collection**  
   Employee data extracted with fields: `Gender`, `Age`.

2. **Data Cleaning**  
   - Handled missing values
   - Formatted entries for consistency

3. **Age Grouping Logic**  
```python
bins = [0, 20, 30, 40, 50, 100]
labels = ['<20', '20–30', '30–40', '40–50', '50+']
df['Age Group'] = pd.cut(df['Age'], bins=bins, labels=labels)
