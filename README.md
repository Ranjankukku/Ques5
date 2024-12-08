# Ques5

Below are the full questions and their corresponding answers based on the provided document.

---

### **Question 1(a):**
You are asked to plan a data analytics project to analyze student feedback to DCU in relation to online teaching in 2020 and 2021. Using the Generic Data Analytics Pipeline discussed in CA682, assign each of the following activities to one of the 5 main categories: Gathering, Processing, Analyzing, Presenting, and Preserving. Identify a tool or application that you might use (same one can be used for multiple tasks).

1. Documenting the data formats used in the study and saving all of the created datasets.
   - **Category:** Preserving
   - **Tool:** Microsoft Excel or Google Sheets

2. Removing incorrect entries from the student datasets.
   - **Category:** Processing
   - **Tool:** Python (using Pandas library)

3. Liaising with DCU Registry to get datasets from the student registration and results systems.
   - **Category:** Gathering
   - **Tool:** SQL or email communication tools

4. Calculating the average satisfaction levels based on the sentiment ratings.
   - **Category:** Analyzing
   - **Tool:** Python (using NumPy or Pandas)

5. Anonymizing student comments that include identifying details.
   - **Category:** Processing
   - **Tool:** Python (Natural Language Processing libraries)

6. Converting student words into sentiment ratings and correlating with field of study.
   - **Category:** Analyzing
   - **Tool:** Python (NLTK or TextBlob)

7. Conducting student surveys to answer the key questions about their experience.
   - **Category:** Gathering
   - **Tool:** Google Forms or SurveyMonkey

8. Creating a document to share with senior university management summarizing the findings.
   - **Category:** Presenting
   - **Tool:** Microsoft PowerPoint or Tableau

---

### **Question 1(b):**
Identify a weakness (or important task that is not included) with the Generic Data Analytics Pipeline.

- **Answer:** A key weakness of the Generic Data Analytics Pipeline is that it does not explicitly address *data governance* or *ethical considerations*, such as ensuring compliance with GDPR regulations or managing consent for data usage.

---

### **Question 1(c):**
For each of the following data attributes (A-D), choose all applicable descriptions: Qualitative, Quantitative, Discrete, Continuous, Nominal, Ordinal, Interval, Ratio.

A. Rating of temperature comfort in offices (cold, cool, perfect, warm, hot)
- Qualitative
- Ordinal

B. Number of times a character's name is used in a TV show episode
- Quantitative
- Discrete
- Ratio

C. Names of pets owned by all CA682 students
- Qualitative
- Nominal

D. All winning times (in seconds) for men's 100m sprint at the Olympic Games
- Quantitative
- Continuous
- Ratio

---

### **Question 1(d):**
Choose one scenario and explain why it is or is not a good example of "big" data according to the three classical characteristics (Volume, Velocity, Variety). State any assumptions about the data and its characteristics.

**Scenario B: An individual's step count data for a 1-year period from a personal smart device (e.g., Fitbit)**

- This is *not* a good example of big data because:
  - The volume of data is relatively small as it pertains to a single individual.
  - The velocity is low since step counts are recorded periodically rather than in real-time streams.
  - The variety is limited as it only includes step counts without additional diverse datasets.

Assumption: The dataset contains only step counts without integration with other metrics like heart rate or location.

---

### **Question 2(a):**
Given the brief for designing a system for integrating inventory and sales data:

(i) List three important questions you would ask your client about their data storage requirements.

1. What is the expected volume of daily transactions across all stores?
2. What level of access control and security is required for sensitive sales data?
3. Are there any specific reporting or analytics tools that need to integrate with this system?

(ii) Suggest a type of data storage approach to use for this project, giving a reason for your choice.

- Relational Database Management System (RDBMS), such as MySQL or PostgreSQL, because it can handle structured sales and inventory data efficiently while supporting complex queries.

(iii) The client now wants to include website logs and social media content interactions. Would this change your recommendation? Why/Why not?

- Yes, this would change the recommendation to a hybrid approach combining RDBMS for structured data and NoSQL databases like MongoDB for unstructured web logs and social media interactions. This ensures scalability and flexibility for diverse data types.

---

### **Question 2(b):**
(i) Give three examples of simple metadata describing your favorite item of clothing.

1. Color: Blue
2. Size: Medium
3. Material: Cotton

(ii) For each metadata element, identify if it is Descriptive, Administrative, or Structural and briefly explain why.

1. Color: Descriptive – It provides information about appearance.
2. Size: Descriptive – It describes physical dimensions.
3. Material: Descriptive – It specifies composition details.

(iii) How would using a standard improve metadata quality? Identify one potential difficulty with enforcing it.

- Using a standard ensures consistency and interoperability across datasets. A difficulty could be resistance from users unfamiliar with standardized formats or requiring legacy system updates.

---

### **Question 2(c):**
Identify any possible data that may need to be handled differently due to European GDPR requirements.

- Social media interactions may include personal identifiers such as usernames or comments tied to individuals. These must be anonymized or pseudonymized under GDPR regulations to protect user privacy.

---

### **Question 3(a):**
Identify four possible errors or artifacts in the dataset linked above:

1. Missing values in production columns (e.g., blank cells).
2. Outliers such as negative production values.
3. Duplicated rows for certain countries/years.
4. Incorrect date formatting in year columns.

**Tool Used:** Microsoft Excel / Python (Pandas).

---

### **Question 3(b):**
How were these errors introduced?

1. Missing values: Likely during *Gathering* due to incomplete reporting by countries.
2. Negative values: Introduced during *Processing* due to manual entry errors.
3. Duplicates: Resulted from *Gathering* when merging multiple sources without deduplication.
4. Date formatting issues: Occurred during *Processing* when converting formats inconsistently.

---

### **Question 3(c):**
What methods would you suggest to mitigate errors?

1. Use validation rules during data entry to prevent negative values.
2. Implement automated deduplication scripts during processing.
3. Standardize date formats using consistent parsing methods.
4. Conduct completeness checks during gathering phases.

These methods improve accuracy and consistency across datasets.


### **Question 4(a):**  
**Is this an exploratory or explanatory visualisation task?**  
- **Answer:** This is an explanatory visualisation task because the goal is to communicate specific findings (e.g., 60% of students live within 10 km of the Glasnevin campus) to senior university management.

---

### **Question 4(b):**  
**Who is the intended audience for the data visualisation?**  
- **Answer:** The intended audience is senior university management at DCU, who need a clear and concise summary of student accommodation trends to inform decision-making.

---

### **Question 4(c):**  
**What title might you give to the data visualisation and why? Make assumptions about any conclusion.**  
- **Answer:** A suitable title could be: *"Student Accommodation Trends: Proximity to Glasnevin Campus and Rent Distribution"* because it highlights both key aspects of the analysis—geographical distribution and median rent trends.

---

### **Question 4(d):**  
**What specific chart type would you use? Justify your choice referring to the principles discussed in class relating to data types and the message.**  
- **Answer:** A combination of a bar chart and a map would be ideal:
  - A bar chart can display the number of students or percentage distribution across distance categories.
  - A geographical map can visually represent where students live relative to the Glasnevin campus.  
This approach aligns with principles of clarity and relevance, as it uses appropriate visual encodings for categorical and spatial data.

---

### **Question 4(e):**  
**For your data visualisation, what marks and attributes will you use to encode the data? Be specific about the values of the attributes.**  
- **Answer:**  
  - **Marks:** Bars for numerical data (e.g., number of students) and points for geographical locations on a map.  
  - **Attributes:**
    - Height of bars: Encodes the number/percentage of students.
    - Color intensity on map: Represents density of student accommodation in different areas.
    - Labels: Display exact values (e.g., median rent or percentage).

---

### **Question 4(f):**  
**Considering the purpose and intended audience, comment on how you would use colour or layout principles for this data visualisation.**  
- **Answer:**  
  - Use a consistent color palette with distinct but harmonious shades for each distance category (e.g., light blue for closer distances, darker shades for farther distances).  
  - Ensure high contrast between text and background for readability.  
  - Place key findings (e.g., "60% live within 10 km") prominently at the top or center of the visualisation.  

---

### **Question 5(a):**  
**Identify three possible improvements that you could make to the graph below. Justify your choices, referencing design rules and theories.**

1. **Remove unnecessary 3D effects:** The 3D design adds clutter without improving understanding; a flat design would be clearer.
2. **Add data labels:** Include exact values on each segment to improve precision and reduce reliance on estimation.
3. **Use a consistent color scheme:** Avoid overly bright or clashing colors; use a cohesive palette aligned with accessibility standards.

---

### **Question 5(b):**
**Given the following visualisation tasks, suggest an appropriate graph type (specific chart type and CHRTS category) for each to display the information and give a brief justification.**

A. Compare the performance of stocks in Microsoft, Apple, and Samsung over the last 5 years.
- **Graph Type:** Line chart (CHRTS category: Trend).  
- **Justification:** A line chart effectively shows changes over time, making it easy to compare stock performance trends.

B. Explore movie commercial performance for IMDB top 50 by director based on cost to make and ticket sales.
- **Graph Type:** Scatter plot (CHRTS category: Relationship).  
- **Justification:** A scatter plot allows comparison between two continuous variables (cost vs ticket sales), revealing patterns or outliers.

---

### **Question 5(c):**
**Answer the following questions relating to the graphic shown below:**

(i) What is the main communication purpose and why?  
- **Answer:** The main purpose is explanatory—it aims to highlight specific relationships or insights about the dataset in a clear and focused manner.

(ii) What design choices or guidelines have been used to support this purpose?  
- **Answer:** The graphic likely uses:
  - Clear axis labels to define variables.
  - Appropriate scaling to ensure accurate interpretation.
  - Minimalistic design elements to avoid distractions while emphasizing key insights.

--- 

This completes all questions from the provided document! Let me know if further clarification is needed!


<img width="1470" alt="Screenshot 2024-12-08 at 5 16 20 PM" src="https://github.com/user-attachments/assets/d86bf88c-d10a-424b-a047-228a07b5bed6">
<img width="1470" alt="Screenshot 2024-12-08 at 5 16 17 PM" src="https://github.com/user-attachments/assets/19fd2e3d-e4e4-49c3-bf93-9cadd8a5582a">
<img width="1470" alt="Screenshot 2024-12-08 at 5 16 12 PM" src="https://github.com/user-attachments/assets/86a7baa8-d5c0-437f-a31c-20d602e09bfc">
<img width="1470" alt="Screenshot 2024-12-08 at 5 16 09 PM" src="https://github.com/user-attachments/assets/2e569c7f-e7fd-4dc2-a986-552d8793c997">
<img width="1470" alt="Screenshot 2024-12-08 at 5 16 03 PM" src="https://github.com/user-attachments/assets/59bb05c2-70ac-4e83-a5b2-9bc93ec941c8">
<img width="1470" alt="Screenshot 2024-12-08 at 5 15 51 PM" src="https://github.com/user-attachments/assets/3cd33de9-9e9b-4191-9d81-b538bb2b75cd">
<img width="1470" alt="Screenshot 2024-12-08 at 5 15 08 PM" src="https://github.com/user-attachments/assets/4d6cf95a-3c51-434a-9e45-67446c16f4e5">
<img width="1470" alt="Screenshot 2024-12-08 at 5 15 03 PM" src="https://github.com/user-attachments/assets/2f902d2c-9544-4556-911f-c17fbca579b1">
