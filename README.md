![MasterHead](https://buzzrx.s3.amazonaws.com/0df5d5b0-3a24-47e6-b362-27511aa23517/MedSideEffects.png)

# Drugs, Side Effects, and Medical Condition
This project revolves around the different medical conditions and the drugs related to cure them

---

## 🎯 Aim of the Project
This project is specified towards the different diseases, medical conditions, and symptoms that are showed when someone falls ill. It also prescribes the drugs related to specific medical conditions and what could be the possible side effects that would arise if taken in incorrect manner.

---

## 🖊️ Objectives
1. Analyze the Relationship Between Drugs, Medical Conditions, and Side Effects:</br>
To understand how specific drugs are associated with particular medical conditions and identify common or severe side effects. This involves parsing textual data and quantifying relationships, which helps in determining drug efficacy and risk.
</br>

2. Perform Exploratory Data Analysis (EDA):</br>
To use EDA techniques (e.g., histograms, boxplots, heatmaps) to visualize trends, distributions, and patterns in the dataset. This includes analyzing:</br>
- Ratings distribution</br>
- Side effect frequency</br>
- Most common conditions treated</br>
</br>

3. Identify the Most Commonly Used Drugs per Condition:</br>
To group and rank drugs based on the frequency of their use in treating particular medical conditions (e.g., Acne, Pain, Diabetes). This helps in understanding drug popularity and prescribing patterns.
</br>

4. Investigate High-Risk Side Effects:</br>
To isolate and track severe or frequently occurring side effects (e.g., hives, difficulty breathing). This objective supports public health and pharmaceutical research by identifying drugs with high adverse effect rates.
</br>

5. Classify and Count Drug Categories:</br>
To extract and count how often each drug class appears (e.g., antibiotics, antihistamines, topical steroids). This provides insights into which drug classes are prevalent for specific conditions or side effects.
</br>

6. Examine Drug Safety Based on Pregnancy Categories:</br>
To evaluate the risk profiles of drugs during pregnancy (Categories A to X, and N/Unknown). This objective helps in understanding which drugs are safer or riskier for pregnant patients.
</br>

7. Assess Prescription Type Distribution (Rx/OTC):</br>
To determine how many drugs are Prescription-only (Rx), Over-the-Counter (OTC), or both (Rx/OTC). This gives regulatory and accessibility insights into medication availability.
</br>

8. Measure Drug Effectiveness Using Ratings and Reviews:</br>
To analyze average user ratings and number of reviews for each drug, which indicates perceived effectiveness, satisfaction, and usage popularity. Useful for comparing patient-reported outcomes.
</br>

9. Understand Drug Abuse Potential (CSA Classification):</br>
To classify drugs based on their Controlled Substances Act (CSA) Schedule (1–5, N, U, M), helping identify those with high abuse potential versus safer alternatives.
</br>

10. Prepare the Dataset for Machine Learning Models:</br>
To clean, encode, and scale the dataset using preprocessing steps like:</br>
- Label encoding categorical values (e.g., side effects, CSA, Rx_OTC)</br>
- Handling missing data</br>
- Feature scaling for modeling tasks like clustering or classification</br>
- This ensures the data is ready for building predictive models or rule-mining (e.g., Apriori).</br>

---

## 🔑 Key Processes
1. Data Collection and Understanding:</br>
- Source: The dataset was collected from public databases like drugs.com and Kaggle.
- Content Overview: It contains 17 columns and over 2,900 rows detailing drug names, associated medical conditions, side effects, drug classes, ratings, pregnancy risk categories, CSA scheduling, and more.
- Objective: To understand the scope of the data — what each column represents, how it contributes to the analysis, and how it can be linked to real-world healthcare insights.
</br>

2. Data Cleaning and Preprocessing:</br>
- Handling Missing Values: Replacing nulls in key columns (side_effects, drug_classes, generic_name, etc.) with placeholders like 'Unknown', 0, or category-appropriate defaults.
- Data Encoding: Applied label encoding to convert categorical data (e.g., pregnancy_category, rx_otc, side_effects) into numerical format for machine learning.
- Feature Transformation: Cleaned the activity column by removing % and converting to float, transformed alcohol column into binary interaction (1 for "interacts", 0 for "no interaction").
- Output: A fully sanitized and numerical dataset ready for analysis and modeling.
</br>

3. Exploratory Data Analysis (EDA) and Visualization:</br>
- Univariate Analysis: Distribution plots of drug ratings, counts of side effects, and CSA schedules to understand individual variable behavior.
- Bivariate Analysis: Boxplots of drug ratings by drug class, frequency comparisons between drug types and medical conditions.
- Frequency Extraction: Used techniques like text parsing and tokenization to extract and count:
- Most common side effects
- Most prescribed drug classes
- Frequently treated medical conditions
- Visualization Tools: Used matplotlib and seaborn to visualize heatmaps, bar graphs, histograms, and distribution curves.
</br>

4. Feature Engineering and Transformation for Modeling:</br>
- Boolean Columns: Created new binary columns to indicate the presence of specific side effects (Hives, Itching, etc.) and conditions (Acne, Pain, etc.).
- Scaling: Applied StandardScaler to normalize the dataset for better model performance.
- Correlation Analysis: Generated heatmaps to visualize interdependencies and identify impactful features.
- Association Rules (Optional): Introduced Apriori algorithm to uncover relationships like “If a drug treats Acne, it is likely to belong to class X and cause side effect Y.”
</br>

5. Result Interpretation and Reporting:</br>
Insights Generated:
- Which drugs are most used for common conditions like Acne or Pain.
- Side effects that are widespread across multiple drugs.
- Ratings trends by drug class or medical condition.
- Deliverables: Cleaned datasets, visual reports (plots, charts), and CSV files summarizing side effect counts, condition frequencies, and drug class distributions.
- Use Cases: Beneficial for healthcare analysts, pharmacologists, and regulatory bodies to understand drug risks, recommend alternatives, or design safer treatment plans.

---

## 🛎️ Important Graphs Related to the project
1. Correlation HeatMap</br>
</br>
<img width="1036" height="810" alt="img_1" src="https://github.com/user-attachments/assets/4adcfcd2-f3c6-44ee-ad07-f9454fe25c16" /></br>
</br>

2. Count of Hives</br>
</br>
<img width="549" height="393" alt="img_2" src="https://github.com/user-attachments/assets/e2c4c4c3-6277-4fa6-9ad6-a54046b49b4f" /></br>
</br>

3. Count of Difficult Breathing</br>
</br>
<img width="549" height="393" alt="img_3" src="https://github.com/user-attachments/assets/b621dc2e-cd28-4616-9fae-d927bd966e02" /></br>
</br>

4. Count of Itching</br>
</br>
<img width="549" height="393" alt="img_4" src="https://github.com/user-attachments/assets/16d44572-84d4-431b-809f-a7eec81fa489" /></br>
</br>

5. Count of Upper Respiratory Combinations</br>
</br>
<img width="549" height="393" alt="img_5" src="https://github.com/user-attachments/assets/72eb9919-0d60-4efe-a753-498e07f8dd9e" /></br>
</br>

6. Count of Topical Steroids</br>
</br>
<img width="549" height="393" alt="img_6" src="https://github.com/user-attachments/assets/d4fc87ec-3815-458f-8672-eb734d946bc1" /></br>
</br>

7. Count of Topical Acne Agents</br>
</br>
<img width="549" height="393" alt="img_7" src="https://github.com/user-attachments/assets/9cb87e85-1f8a-44ba-b9b6-11f07ab921a0" /></br>
</br>

8. Distribution of Drug Ratings</br>
</br>
<img width="850" height="547" alt="img_8" src="https://github.com/user-attachments/assets/3e9fc1f0-1e97-440b-bb29-9b5eec63257e" /></br>
</br>

9. Drug Ratings by Class</br>
</br>
<img width="1002" height="1614" alt="img_9" src="https://github.com/user-attachments/assets/47520170-0d0c-4b2f-92a7-f6713a7f5f76" /></br>
</br>

---

## 📩 Conlcusion
This project offered a comprehensive data-driven analysis of the intricate relationships between various pharmaceutical drugs, their associated medical conditions, and the side effects they may cause. By leveraging Python-based data analytics, visualization, and preprocessing techniques, the project provided meaningful insights into the real-world implications of drug usage and safety, particularly from the perspective of patients and healthcare professionals. We began by understanding the structure and scope of the dataset, which contained 17 critical attributes, including drug names, medical conditions, user ratings, side effects, and regulatory classifications such as pregnancy categories and CSA schedules. After carefully cleaning and preparing the dataset — including handling missing values and transforming categorical features — we conducted in-depth exploratory data analysis (EDA) to uncover hidden trends and patterns. The results were illuminating. The analysis revealed that drugs like those used for Pain, Acne, and Colds & Flu are among the most frequently prescribed. Hives, difficult breathing, and itching emerged as the most common side effects, while Topical acne agents and Upper respiratory combinations dominated drug class usage. These insights not only reflect the prevalence of certain health conditions but also raise critical considerations regarding patient safety and drug effectiveness. In addition, the study explored how ratings and reviews vary across different drug classes and conditions, providing a user-centered perspective on drug efficacy. The integration of data on pregnancy risks and substance abuse potential further enriched the analysis by adding layers of medical and regulatory insight. Ultimately, this project demonstrates the power of data analytics in healthcare, especially in guiding clinical decisions, improving pharmacovigilance, and supporting public health policies. It also sets a foundation for future enhancements through machine learning models, predictive analysis, and recommendation systems, potentially leading to smarter, safer, and more personalized treatment strategies.

---

## ✍️ Key Learnings from this Project
The project emphasized the usefulness of feature engineering and transformation, including label encoding and standardization, which prepared the dataset for further statistical or machine learning applications. Learning how to create binary indicators for specific side effects or drug classes taught us how raw data can be refined to serve deeper analytical goals. Additionally, working with healthcare-related data helped build an understanding of real-world pharmaceutical classifications, such as pregnancy categories, CSA schedules, and Rx/OTC statuses. These concepts added context to our data and improved our domain knowledge—an essential skill when dealing with specialized industries like healthcare. Lastly, the project demonstrated how data science can directly contribute to public health and medical decision-making. By identifying frequently used drugs, commonly reported side effects, and drugs with higher ratings, we were able to simulate how analytics can aid in choosing safer, more effective medications. This project reinforced the power of data in making healthcare smarter, safer, and more patient-centered.
