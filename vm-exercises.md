# Virtual Machine (VM) Exercises

## :information_source: Read this before getting started
- The two exercises should not replicate the exact actions shown in your screencast. The goal of exercises is for learners to apply what was learned in the screencasts to new problems or situations. This is best pedagogical practice for retaining and building skills. For example, this can be done by using another dataset between screencasts and exercises or focusing on a different portion of the dataset.
- Power BI / Tableau specific: We can only run free versions of BI software in our virtual machine exercises. In the case of Power BI, make sure the exercises can run on [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) without any additional paid products. 
- Unsure what the scope of an exercise should be? Here's an [example](https://campus.datacamp.com/courses/introduction-to-power-bi/getting-started-with-power-bi?ex=14) from Introduction to Power BI. The first chapter of most DataCamp courses are free, so take a look at our [BI courses](https://learn.datacamp.com/courses?technologies=Tableau&technologies=Power%20BI) to get a feel for how we assess and guide learners.

## 1st VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder - Done

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-1-intial.twbx` or `ex-1-intial.pbix` or `ex-1-initial.yxmd`, depending if you are auditioning for a Tableau/Power BI/Alteryx course.
- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-1-sol.twbx` or `ex-1-sol.pbix` or `ex-1-sol.yxmd`

#### Learning Objective

Learners will create dropdown menus in Excel for the "Audio Equipment," "Computers," and "Outdoor" categories by referencing a predefined range of items in the worksheet.

#### Context

You are creating a system for managing product categories where dropdowns will reference a range of predefined items. This ensures dynamic updates if the source list changes.

#### Steps to be executed by the student (max 6)

Step 1: Open the provided "ex-1-intial.xlsx" file.

Step 2: Highlight cells I2:I6 (under "Audio Equipment").
Step 3: Go to the Data tab, select Data Validation, and choose the List option.
Step 4: In the Source box, enter the range where "Audio Equipment" items are located, e.g., =$C$2:$C$6.
Step 5: Repeat steps 3 and 4 for Computers & Outdoors Subcategory.
Step 6: Save your changes.

#### Exercise question:
Question:
What happens if you add a new item to the "Audio Equipment" list in cell C7?

Correct Answer:
The dropdown will not include the new item unless the range is updated to include the additional row.

#### End goal:

![image](https://github.com/user-attachments/assets/241a7cc8-196a-4408-8f7f-af234e1d3845)

## 2nd VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder - Done/Same Dataset

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-2-intial.twbx` or `ex-1-initial.yxmd`, depending if you are auditioning for a Tableau/Power BI/Alteryx course.
- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-2-sol.twbx` or `ex-2-sol.pbix` or `ex-1-sol.yxmd`

#### Learning Objective

Learners will create dependent dropdown menus using the INDIRECT formula to dynamically display items based on a parent category.

#### Context

You are designing an inventory form for your store. Users will first select a main category (e.g., Furniture, Clothing, Kitchen), and based on their selection, a second dropdown will show relevant subcategories.

#### Steps to be executed by the student (max 6)

Step 1: Open the provided "ex-2-intial.xlsx" file.
Step 2: Define the named ranges for all the categories given on the "Category Details" sheet: Example:
B2:B5 as "Furniture"
C2:C5 as "Clothing"
D2:D5 as "Kitchen"
Step 3: In cell H1, create a dropdown for the categories: Furniture, Clothing, Kitchen using Data Validation.
Step 4: In cell I1, create a dependent dropdown using the formula: =INDIRECT(H1). Repeat the same for others.
Step 5: Test your dropdowns: Select an item in H2. Ensure that the dependent dropdown in I2 shows the correct subcategories. 
Step 6: Save your changes.

#### Exercise question:
Question:
What happens in cell I1 if the category in cell H1 is cleared?

Correct Answer:
The dependent dropdown in I1 will remain empty.

#### End goal:

![image](https://github.com/user-attachments/assets/05bb043b-5f9c-4697-adb4-83caadb66433)


