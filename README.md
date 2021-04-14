# Hi 👋, I'm Ranveer Singh
<br>

## Task
### Self and others Evaluation and make a report in SpreadSheets
#### Details of Task 
- Create a spreadsheets of all interns with some key points and give a ratings on all key points in Poor, Fair, Satisfactory, Good, Very good, Excellent
- Set a formula to get avarage in avarage columns
- Set another formula to get entire row  colour **Red** if avarage value equal to or less then 2.5

## Test Case
| Task | Desired Output | Actual Output  | Test Status |
|------|----------------|----------------|-------------|
| Set a formula to get avarage in avarage columns | Get exect avarage in avarage columns | getting exect avarage in avarage columns | Pass |
| Set a formula to get entire **row**  colour **Red** if avarage value equal to or less then 2.5 | Row  colour **Red** if avarage value equal to or less then 2.5 | Only avarage **columns Red** if avarage value equal to or less then 2.5 | Fail |

## Formula used To get the Desired Output
### A.) Get exect avarage in avarage columns
```sh
=ArrayFormula(SUM(COUNTIF(Cn:Jn,{"Excellent","Very good","Good","Satisfactory","Fair","Poor"})*{5,4,3,2,1,0}))/COUNTA(Cn:Jn)
```
```sh
Note- Cn:Jn (n is the No. of columns)
```
#### Explanation of formula 
- **_Array Function_**
```sh
"An array function is a function that can perform multiple calculations on one or more items in an array."
```
- **_SUM_**
```sh
"The SUM function adds values. You can add individual values, cell references or ranges or a mix of all three. For example: =SUM(A2:A10) Adds the values in cells A2:10."
```
- **_COUNTIF_**
```sh
"Returns the count of a range depending on multiple criteria."
```
- **_COUNTA_**
```sh
"Returns the number of values in a dataset."
```
### B.) Set another formula to get entire row  colour **Red** if avarage value equal to or less then 2.5

- open a spreadsheet in Google Sheets.
- Select the cells you want to apply format rules to.
- Click Format and then Conditional formatting. A toolbar will open to the right.
- Create a rule.
- In rule condition select less then or equal to 2.5
- Select colour Red
- Single color: Under "Format cells if," choose the condition that you want to trigger the rule. Under "Formatting style, choose what the cell will look like when conditions are met.
- click the Down arrow Down Arrow.
- Click Done.



