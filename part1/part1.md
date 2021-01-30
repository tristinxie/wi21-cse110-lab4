1. The size of the prices array will be printed to the console because the for loop iterator `i` used the `var` declaration keyword. This causes `i` to be hoisted to the top of the function and ignores codeblocks.
2. A number will be printed to the console with similar reasons from question 1. The `discountedPrice` variable was declared with `var` which hoists it to the top of the function and ignores codeblocks.
3. The same number will be printed to console as questions 2 and it will be the last discounted price of the prices array. `finalprice` is already at the top of the function so it being hoisted doesn't change functionality but it does happen because it was declared with `var`
4. [ 50, 100, 150 ] will be returned. We pass the `prices` array and the 0.5 float `discount` value into the function. We create `discounted` array and `finalPrice` int value. We loop through the `prices` array and calculate the discounted price for each item in the `prices` array and push it into the `discounted` array. After all of this is done, we return the `discounted` array with all the discounted prices.
5. We will get a ReferenceError because `i` refers to a variable in the `for` codeblock that was declared using `let` which can only be referenced in its own scope and not outside of the `for` codeblock in the function.
6. We will again get a ReferenceError since the console log can't access the variable that was declared in the `for` codeblock's scope because we declared the variable on this line with `let` keyword.
7. If we don't consider the lines above which will throw errors, then this line in isolation will print the last value in the `discounted` array which is the `finalPrice` of the last item. This is because `finalPrice` was declared in the function's scope, on the same scope as the console log. Although we modified it in the for loop, where it is declared determines the scope.
8. [ 50, 100, 150 ] will be returned. We pass the `prices` array and the 0.5 float `discount` value into the function. We create `discounted` array and `finalPrice` int value. We loop through the `prices` array and calculate the discounted price for each item in the `prices` array and push it into the `discounted` array. After all of this is done, we return the `discounted` array with all the discounted prices.
9. Assuming we ignore the assignment to constant variable error on line 7, we will get a ReferenceError since we used the `let` keyword to declare the iterator `i` in the for loop codeblock. The `let` declaration keyword only allows code within the same scope to assess the variable.
10. Assuming we ignore the assignment to constant variable error on line 7, we will get a ReferenceError since we used the `const` keyword to declare `discountPrice` in the for loop codeblock. The `const` declaration keyword only allows code within the same scope to assess the variable.
11. We will get an assignment to constant variable error on line 7, because we declared `finalPrice` with the `const` keyword at the beginning of the function. So when we go to reassign it in the for loop it throws the error because `const` variables should remain constant and not be reassigned.
12. Assuming we ignore the assignment to constant variable error on line 7, [ 50, 100, 150 ] will be returned. We pass the `prices` array and the 0.5 float `discount` value into the function. We create `discounted` array and `finalPrice` int value. We loop through the `prices` array and calculate the discounted price for each item in the `prices` array and push it into the `discounted` array. After all of this is done, we return the `discounted` array with all the discounted prices.
13. A. `student.name;` <br>
B. `student['Grad Year'];` <br>
C. `student.greeting();` <br>
D. `student['Favorite Teacher'].name;` <br>
E. `student.courseLoad[0];`
14. A. Output: `'32'` the string '3' makes JavaScript convert 2 to a string and concatenate it with '3' to make '32'.<br>
    B. Output: `1` since there is no string operator for `-`, it converts '3' to a number and subtracts with 2<br>
    C. Output: `3` we get a number because `null` converts to 0 and is added to 3<br>
    D. Output: `'3null'` the '3' is a string which causes `null` to be converted to a string and they get concatenated<br>
    E. Output: `4` the boolean value of `true` is converted to a 1 when adding with a number<br>
    F. Output: `0` both `false` and `null` values are converted to the value 0 and summed to get 0.<br>
    G. Output: `'3undefined'` since the string "3" causes `undefined` to be converted to a string and then concatenated <br>
    H. Output: `NaN` when subtracting it converts "3" to a number but `undefined` becomes `NaN` which when subtracted is still `NaN`<br>
15. A. Output: `true` since '2' get converted to a number and 2 is greater than 1 <br>
        B. Output: `false` since this a comparison of strings and the '2' is greater than the '1' in '12' in Unicode order<br>
        C. Output: `true` the '2' gets converted to a number and both are 2 <br>
        D. Output: `false` we are using strict equality here and since its comparing different types it returns false<br>
        E. Output: `false` the boolean `true` gets converted to a 1 and that isn't equal to 2<br>
        F. Output: `true` we are using strict equality and both are the same types. The Boolean of 2 becomes true because it isn't 0, thus both are true and equal<br>
16. The regular equality check == check equality but tries to convert the values of different types being compared so that they could be compared. The strict equality operator === on the other hand checks equality and returns false if the types being compared aren't the same.
17. `'How are you'` gets printed because `2 == true` returns `false` when the right hand side `true` gets converted to a 1 and isn't equal to 2. Then the `else if(2)` statement is true because any number that isn't 0 is true, so the console log within this condition is printed.
18. In seperate file.
19. [ 6, 8, 10 ] is outputted. When we call `modifyArray` with [ 1, 2, 3 ] and `doSomething` as parameters, we first created a new storage array. Then for each number in [ 1, 2, 3 ] we call the `callback` parameter which is the same as `doSomething` and pass in the current number at `i` in our [ 1, 2, 3 ] array and a function that multiplies a parameter by 2. Inside the `doSomething` function, we return the result of the callback which is now the function we just passed in that multiplies by 2. However, we pass in the function the number added by 2. So each number that gets pushed in the `newArr` is has 2 added to it first then multiplied by 2. The result is informally expressed like this: [ (1+2)*2, (2+2)*2, (3+2)*2 ] so we get [ 6, 8, 10 ].
20. In seperate file.
21. `1 4 3 2` gets outputted.