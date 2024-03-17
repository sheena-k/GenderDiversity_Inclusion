# Diversity_Inclusion
---
**The purpose of this analysis is to:**

* **Define proper KPIs in hiring, promotion, performance, and turnover.**
  
* **Create a visualization for the HR manager that reflects all relevant Key Performance indicators(KPIs) and metrics in the dataset.**
---
![GitHub Logo](https://github.com/sheena-k/Gender_Diversity_Inclusion/blob/main/task4.png)
---
## Data Analysis Xpression (DAX):
---
* **Female % = DIVIDE([Female Count], [Total Gender Count])**

* **Male % = DIVIDE([Male Count], [Total Gender Count])**

* **% employees promoted (FY21) = Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[Promotion in FY21?]="Yes")),Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[In base group for Promotion FY21]="Yes")))**
  
* **% Promotees who were men = Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[Gender]="Male")),distinctcount('Pharma Group AG'[Employee ID]))**
  
* **% Promotees who were women = Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[Gender]="Female")),distinctcount('Pharma Group AG'[Employee ID]))**
  
* **% Turnover = Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[FY20 leaver?]="Yes")),Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[In base group for turnover FY20]="Y"))+Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG',NOT('Pharma Group AG'[Department @01.07.2020]=BLANK()))),2))**

## Inferences:
---
* **Empowering diversity and gender equality is key to achieving a balanced workforce. According to the given dataset, 59% (295) of employers are male, and 41% (205) are female. Encouraging a workplace with a 50-50% gender ratio should be prioritized; however, hiring should be based on competency rather than gender.**


* **According to company records, in the fiscal year FY21, 14% of promotions were given to men, and 12% to women. Despite the better performance of female directors, there remains a significant gender imbalance in the distribution of new hires and promotions for executive positions.**


* **In general, promotions are based on experience, with individuals aged 30 to 49 being promoted to higher job positions. The majority of individuals in the age group 20 to 29 hold junior officer-level jobs.**


* **For individuals above the age of 49, no inference can be drawn from the collected samples of data.**


Overall, there is diversity in performance ratings across different age groups.
