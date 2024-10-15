# BOOLEAN_FUNCTION_MINIMIZATION

```
Developed by: Oswald Shilo
Reg No: 212223040139
```

## **AIM:**
To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## **Equipment Required:**

**Hardware – PCs, Cyclone II , USB flasher**

**Software – Quartus prime**

## **Theory**:
* Boolean Function Minimization:
Simplifies Boolean expressions to optimize hardware design and improve efficiency.

* Logic Gates:
Boolean expressions are realized using fundamental logic gates like AND, OR, and NOT.

* Verilog:
A hardware description language used to model, simulate, and synthesize digital circuits.

* Quartus Software:
Used for designing, compiling, and verifying FPGA implementations of logic functions.

* RTL Schematic:
Displays the hardware structure of the Boolean function, helping in understanding the circuit's operation.


## **Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## **Program:**

##### Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

```
module ex2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule
```

```
module ex2m2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```



## **Truth Table:**

![2 1 truth table](https://github.com/user-attachments/assets/6a3f7a61-4175-4183-bb22-e91ce1e5bfea)
![2 2 truth table](https://github.com/user-attachments/assets/a94b9962-e99c-4028-a265-5c906cca8121)


## **RTL**
![image](https://github.com/user-attachments/assets/0b616916-2bcd-4b3f-b204-8ee8d662b71d)
![image](https://github.com/user-attachments/assets/94112fb2-d4d7-41d2-a6e8-1385670fe380)


## **Timing Diagram**
![image](https://github.com/user-attachments/assets/5c2f70fe-3c62-474a-a2a5-f4a59318c48f)
![image](https://github.com/user-attachments/assets/bab2bc55-4617-46aa-8786-fbb0f76f4c24)


## **Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

