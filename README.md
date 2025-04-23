# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions.

**Logic Diagram**
![image](https://github.com/user-attachments/assets/7b7eaee9-fbe7-4fbb-bd33-27e118759eee)

**F1**
![image](https://github.com/user-attachments/assets/5ca62fb9-bc69-48c7-a74d-05f7d8ae0614)

**F2**
![image](https://github.com/user-attachments/assets/71c194ce-6fcf-487b-ab22-ba404e34fb8e)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:MAGATHI D
RegisterNumber:212223040108

F1:
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

F2:
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

*/


**RTL realization**
F1:
![image](https://github.com/user-attachments/assets/974a695e-2f86-40b2-94ec-043d8366dba7)


F2:
![image](https://github.com/user-attachments/assets/6ef1f383-c405-49a4-a906-ecf1f5d475bf)

**Timing Diagram**
F1:
![image](https://github.com/user-attachments/assets/1442af83-1c50-47c5-9f68-a2d61fe9228a)

F2:
![image](https://github.com/user-attachments/assets/74c74d74-5daf-4b87-8682-82d77fc92de2)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

