# Global Nuclear Arsenal Expansion Analysis

## 👤 Author

| Name            | Role              | LinkedIn                                      |
|-----------------|-------------------|-----------------------------------------------|
| Jason Emmanuel  | Data Analyst | [linkedin.com/in/jasoneml](https://www.linkedin.com/in/jasoneml/) |

## 📘 Overview

This project investigates the global expansion of nuclear arsenals using historical and current data on nuclear weapons testing, stockpiling, and proliferation. The analysis highlights how trends in nuclear armament impact global security and efforts at disarmament.

The project is based on publicly available datasets and includes exploratory data analysis (EDA), data visualization, and statistical insights into nuclear weapons consideration, pursuit, and possession across countries from 1938 to 2022.

---

## 📊 Datasets

1. **nuclear_weapons_tests_states.csv**  
   - Nuclear tests by country and year.  
   - Columns: `country_name`, `year`, `number_of_tests`.

2. **nuclear_weapons_stockpiles.csv**  
   - Stockpile data showing number of nuclear warheads.  
   - Columns: `country_name`, `year`, `stockpile_total`.

3. **nuclear_weapons_proliferation_total_owid.csv**  
   - Aggregated proliferation trends across entities.  
   - Columns: `entity_name`, `year`, `consideration`, `pursuit`, `possession`.

4. **nuclear_weapons_proliferation_owid.csv**  
   - Detailed entity-level proliferation records.  
   - Columns:
     - `country_name`
     - `year`
     - `nuclear_weapons_status` (0 = None, 1 = Consideration, 2 = Pursuit, 3 = Possession)
     - `nuclear_weapons_consideration`
     - `nuclear_weapons_pursuit`
     - `nuclear_weapons_possession`

---

## 🚀 Features

- Cleaned and preprocessed nuclear proliferation data from 1938 to 2022
- Unique country-year analysis of nuclear activity phases
- Distribution of weapon status across time
- Identification of active proliferation trends and potential global threats
- Statistical summary and missing value report
- Visualizations (bar charts, time-series plots)

---

## 📊 Visualizations

![image](https://github.com/user-attachments/assets/60f62e0b-f020-4011-9db4-7ad75e64b533)

The graph illustrates the cumulative number of countries that have possessed nuclear weapons from 1938 to 2022. It shows a gradual increase starting from the 1940s, with sharp rises during the 1950s to 1980s—a period coinciding with the Cold War—indicating more nations developing nuclear capabilities. The count peaks at 9 around the late 1980s, then slightly drops in the 1990s, reflecting disarmament or denuclearization by some states. It stabilizes again at 9 in the 2000s, suggesting no new countries have acquired nuclear weapons since then, highlighting a plateau in nuclear proliferation.

![image](https://github.com/user-attachments/assets/c5d0f0de-8db9-47e3-8268-52b94afaee09)

This graph displays the trends in three stages of nuclear weapons development—consideration, pursuit, and possession—from 1938 to 2022. The green line indicates the number of countries considering nuclear weapons, which peaked around the late 1960s and then sharply declined, suggesting a decrease in global interest after that period. The yellow line represents countries actively pursuing nuclear weapons, showing sporadic rises through the Cold War era and tapering off significantly after the 1990s. The red line shows nuclear weapons possession, which steadily increased until the late 1980s, plateaued at nine states, and has remained constant since then. This trend reflects the effectiveness of non-proliferation efforts and global treaties in curbing new nuclear states despite historical interest and pursuit.

![image](https://github.com/user-attachments/assets/d797e5d8-10c6-4c93-91e0-a3e70c4e9b05)

This graph illustrates the changes in the number of nuclear warheads possessed globally from around 1945 to 2022. The vertical axis is on a logarithmic scale, indicating a wide range in values. The stockpiles rose dramatically from the early Cold War years, peaking around the late 1980s—reflecting the intense arms race primarily between the United States and the Soviet Union. After the Cold War, a sharp decline in total stockpiles is evident, due to disarmament treaties and arms reduction efforts. Since around 2000, the global stockpile levels appear to have plateaued, indicating stabilization in nuclear arsenals, though they remain in the thousands, highlighting ongoing strategic deterrence postures.

![image](https://github.com/user-attachments/assets/0df920b1-35c9-4f6e-bac3-fb3045b166f3)

The bar chart shows that the United States and Russia conducted the most nuclear tests, with over 1,000 and 700 respectively, reflecting their dominant roles during the Cold War era. France follows at a distant third with around 210 tests, while other nuclear-armed countries like China, the United Kingdom, India, Pakistan, and North Korea have conducted significantly fewer tests. This disparity highlights the historical and geopolitical differences in nuclear weapons development and testing among nations.

---

## 📈 Sample Output

### Status Distribution

| Status Code | Meaning        | Count |
|-------------|----------------|-------|
| 0           | No activity     | 15,797 |
| 1           | Consideration   | 312   |
| 2           | Pursuit         | 236   |
| 3           | Possession      | 503   |

---

## 🛠️ Tools and Libraries Used

| Tools / Libraries   | Description                                             |
|---------------------|---------------------------------------------------------|
| Matplotlib          | Used for creating static, animated, and interactive plots. |
| Pandas              | Used for data manipulation and analysis.                |
| NumPy               | Used for numerical computations and handling arrays.     |
| Seaborn (optional)  | Enhances visualization aesthetics (if used).            |
| Jupyter Notebook    | Interactive environment to write and run Python code.   |

---

## 🔍 How to Use

### Clone the Repository

```bash
git clone https://github.com/your-username/nuclear-analysis.git
cd nuclear-analysis
