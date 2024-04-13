IMPLEMENTATION OF  PL/SQL USING CONDITIONAL STATEMENTS 
 
PROGRAM: 
 
Program to find whether a given number by user is even or odd: 
 
set serveroutput on; 
 
DECLARE  	x int; BEGIN 
	 	x := 15; 
	 	if mod(x,2) = 0 then 
	 	 	dbms_output.put_line('Even Number'); 
	 	else 
	 	 	dbms_output.put_line('Odd Number'); 
	 	end if; 
END; / 
Output: 
Odd Number 
 
Program to find whether the two given numbers are equal and if they are not equal then which one is greater: 
 
set serveroutput on; 
 
DECLARE  	a int;  	b int; BEGIN  	a := 10;  	b := 20;  	if(a>b) then  	 	dbms_output.put_line(‘a is greater than b’);  	elsif(b>a) then  	 	dbms_output.put_line(‘b is greater than a’); 
	 	else 
 	 	dbms_output.put_line(‘Both a and b are equal’);  	end if; 
END; 
/ 
Output: 
b is greater than a 
 
 
Program to demonstrate the use of a simple case statement. 
 
set serveroutput on; 
 
DECLARE 
  grade CHAR(1); BEGIN 
  grade := 'B'; 
 
  CASE grade 
    WHEN 'A' THEN DBMS_OUTPUT.PUT_LINE('Excellent'); 
    WHEN 'B' THEN DBMS_OUTPUT.PUT_LINE('Very Good'); 
    WHEN 'C' THEN DBMS_OUTPUT.PUT_LINE('Good'); 
    WHEN 'D' THEN DBMS_OUTPUT.PUT_LINE('Fair'); 
    WHEN 'F' THEN DBMS_OUTPUT.PUT_LINE('Poor'); 
    ELSE DBMS_OUTPUT.PUT_LINE('No such grade'); 
  END CASE; 
END; 
/ 
Output: 
Very Good 
