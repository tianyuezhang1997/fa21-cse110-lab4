1. Output **3**  
   Because " i " was declared by the keyword " var ", thus the scope of " i " was the whole function. 
2. Output **150**  
   Because " discountedPrice " was declared by the keyword " var ", thus the scope of " discountedPrice " was the whole function. In each iteration of the loop, the value of " discountedPrice " would be updated, and its final value was assigned in the last iteration.  
3. Output **150**  
   Because " finalPrice " was declared by the keyword " var ", thus the scope of " finalPrice " was the whole function. In each iteration of the loop, the value of " finalPrice " would be updated, and its final value was assigned in the last iteration.  
4. Return an array **[ 50, 100, 150 ]**  
   Because " discounted " was declared by the keyword " var ", thus the scope of " discounted " was the whole function. In each iteration of the loop, one half-price element would be pushed into " discounted ", after 3 iterations, " discounted " contained 3 half-price elements.  
5. **ReferenceError: i is not defined**  
   Because " i " was declared by the keyword " let ", thus the scope of " i " was within the " for-loop ".  
6. **ReferenceError: discountedPrice is not defined**  
   Because " discountedPrice " was declared by the keyword " let ", thus the scope of " discountedPrice " was within the " for-loop ".  
7. Output **150**  
   Because " finalPrice " was declared outside the " for-loop ". thus the scope of " finalPrice " was the whole function.
8. Return an array **[ 50, 100, 150 ]**  
   Because " discounted " was declared outside the " for-loop ". thus the scope of " discounted " was the whole function. In each iteration of the loop, one half-price element would be pushed into " discounted ", after 3 iterations, " discounted " contained 3 half-price elements.
9. **ReferenceError: i is not defined**  
   Because " i " was declared by the keyword " let ", thus the scope of " i " was within the " for-loop ".
10. Output **3**  
    Because " length " was declared outside the " for-loop ". thus the scope of " length " was the whole function. Also, the argument " prices " was a array of length 3.   
11. Return an array **[ 50, 100, 150 ]**  
    [ Note that element in " const array " can NOT be reassigned, but pushing new element is always valid ]  
    Because " discounted " was declared outside the " for-loop ". thus the scope of " discounted " was the whole function. In each iteration of the loop, one half-price element would be pushed into " discounted ", after 3 iterations, " discounted " contained 3 half-price elements.   
12. A. student.name  
    B. student['Grad Year']   
    C. student.greeting();   
    D. student['Favorite Teacher'].name   
    E. student.courseLoad[0] 
13. A. **'32'** Because 2 =[String Conversion]=> '2' and concatenate '2' to '3'    
    B. **1** Because '3' =[Numeric Conversion]=> 3 and compute 3 - 2 = 1   
    C. **3** Because 'null' =[Numeric Conversion]=> 0 and compute 3 + 0 = 3     
    D. **'3null'** Because null =[String Conversion]=> 'null' and concatenate 'null' to '3'    
    E. **4** Because 'true' =[Numeric Conversion]=> 1 and compute 1 + 3 = 4     
    F. **0** Because 'false' =[Numeric Conversion]=> 0 and 'null' =[Numeric Conversion]=> 0 and compute 0 + 0 = 0            
    G. **'3undefined'** Because undefined =[String Conversion]=> 'undefined' and concatenate 'undefined' to '3'     
    H. **NaN** Because '3' =[Numeric Conversion]=> 3 but 'undefined' =[Numeric Conversion]=> NaN and compute 3 + NaN = NaN  
14. A. **true** Because '2' =[Numeric Conversion]=> 2 and compare 2 > 1      
    B. **flase** Because they have the same data type, so no type conversion needed, and the first letter of '12' is '1' where '1' is smaller than '2' in Unicode.  
    C. **true** Because '2' =[Numeric Conversion]=> 2 and compare 2 == 2          
    D. **false** Because they have different data type.        
    E. **false** Because 'true' =[Numeric Conversion]=> 1 and compare 1 == 2         
    F. **true** Because 2 was explicitly =[Boolean Conversion]=> true and compare true == true  
15. **===** is a strict equality operator that checks the equality without type conversion.  
    However, **==** is a non-strict equality operator that applies numeric conversion before checking the equality.  
    Especially, the non-strict equality check **==** for **undefined** and **null** is equal without any conversions and do NOT equal anything else.
16. [part2-question16.js](./part2-question16.js)
17. **[ 2, 4, 6 ]** Because the second parameter" callback " of the function " modifyArray " is a function. We passed the function " doSomething " as the second argument, thus each time we execute " callback(array[i]) ", we are calling " doSomething(array[i]) " which returns " array[i] * 2 ". Then push that returning value to the array "newArr". After 3 times of pushing, "newArr" contains 3 elements, and we return it.   
18. [part2-question18.js](./part2-question18.js)
19. **1 4 3 2** Because 3 will be print out at the next event cycle, and there are 1 second delay for printing out 2 
