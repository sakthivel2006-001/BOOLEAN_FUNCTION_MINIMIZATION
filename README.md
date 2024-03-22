# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


module boolean_function(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule 

## Developed by:S.SAKTHIVEL
## RegisterNumber:212223220090


**RTL realization**


![Screenshot 2024-03-22 140917](https://github.com/sakthivel2006-001/BOOLEAN_FUNCTION_MINIMIZATION/assets/151398732/c10aca12-4c3b-43ab-858b-0a65446e54de)



**Truth table:**

![Screenshot 2024-03-22 140145](https://github.com/sakthivel2006-001/BOOLEAN_FUNCTION_MINIMIZATION/assets/151398732/b87a934a-dc4c-4f98-b739-a7352234adf9)


**Timing Diagram**

![Screenshot 2024-03-22 141048](https://github.com/sakthivel2006-001/BOOLEAN_FUNCTION_MINIMIZATION/assets/151398732/c5ddc9d9-18c3-496a-b20e-c123fc6d210c)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

