# Ex. No: 6 PL/SQL program to perform addition and subtraction of two number 
### DATE: 
### AIM: To create PL/SQL program to perform addition and subtraction of two number.

### Steps:
1. Declare the variable a, b and necessary variables in Declare section.
2. Perform addition of two numbers
3. Perform subtraction of two numbers 
4. Display the result 
5. End the begin section.

### Program:
DECLARE
 a NUMBER := 550;
 b NUMBER := 450;
 c NUMBER;
BEGIN
 c:=a+b;
 dbms_output.Put_line('addition of two numbers is '||c);
 c:=a-b;
 dbms_output.Put_line('subtraction of two numbers is '||c);
END;

### Output:
![Screenshot 2024-03-20 120038](https://github.com/ttamizharasi/DBMS/assets/119657317/06f51b2c-4042-4c3b-ada5-4e05b347c70b)


### Result:
Thust the program was performed sucessfully.
