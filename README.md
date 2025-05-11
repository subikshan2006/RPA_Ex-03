```
Name : Subikshan P
Reg.No : 212223240161
```
# RPA_Ex-03
# Aim:
  Get input of name from user and if name is "RAM", Display message as "Welcome Mr. Ramachandran" otherwise "Welcome " followed by Given name. When using Switch case, use different message for every input it gets.

## PROCEDURE:

## 1. Open UiPath Studio:
     Launch UiPath Studio on your system.
## 2. Create a New Project:
            a.Click on "Process".
            b.Give the project a name (e.g., LoopFlowchartDemo).
            c.Click Create.

## 3. Replace Default Sequence with Flowchart:
           a.In Main.xaml, delete the default Sequence activity.
           b.From the Activities panel, drag and drop a Flowchart into the Designer panel.

## A. Repeat (For Each) Loop Section:
         a.Add a Flow Step and rename it as "Start - Repeat".
         b.Add an Assign activity:
            numbers = {1, 2, 3}
            (Create variable numbers of type Integer[] or Array of Int32)
         c.Add a For Each activity:
            *TypeArgument: Int32
            *Values: numbers
            *Inside the For Each, add a Message Box:
               Message: "Repeat: Number is " + item.ToString

## B.While Loop Section:
     a.Add another Flow Step and rename it as "Start - While".
     b.Declare variables:
        countWhile = 1 (Type: Int32)
        max = 3 (Type: Int32)
    c.Add a While activity:
       Condition: countWhile <= max
    d.Inside the While:
        *Add a Message Box:
           Message: "While: Count is " + countWhile.ToString
        *Add an Assign activity:
           countWhile = countWhile + 1

## C. Do While Loop Section:
```
   a.Add a third Flow Step and rename it as "Start - DoWhile".
   b.Declare variable:
      countDo = 1 (Type: Int32)
   c.Add a Do While activity:
      *Condition: countDo <= 3
      *Inside the Do While:
        Add a Message Box: 
           Message: "DoWhile: Count is " + countDo.ToString
        Add an Assign activity:countDo = countDo + 1
```
# Output:
![Screenshot 2025-05-05 103929](https://github.com/user-attachments/assets/2f857faa-fd2e-422a-a737-8269057a2392)
![Screenshot 2025-05-07 212002](https://github.com/user-attachments/assets/1eea243b-986e-4e03-939c-988d8ac2cb3c)

![1](https://github.com/user-attachments/assets/02ad050d-7425-4974-9905-0a6d6b55bbd8)
![2](https://github.com/user-attachments/assets/be23ea47-ec00-4650-bece-ecd3f38b9f9f)
![3](https://github.com/user-attachments/assets/2ff1438b-54aa-4a85-9a3b-0bcfab5582d9)


## Result:
```
When you run the Flowchart:
   1.You will see "Repeat: Number is 1, 2, 3"
   2.Then "While: Count is 1, 2, 3"
   3.Then "DoWhile: Count is 1, 2, 3"
```
