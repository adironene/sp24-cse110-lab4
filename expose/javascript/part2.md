1. line 12 will log 3. We still can refer to var i after the loop exits because the var is declared in the function, so line 12 is within the scope.
2. Line 13 will log 150. the var discountedPrice was last modified during the last iteration of the loop. We assinged it to `prices[i]*(1-discount)` = `300*0.5` = `150`
3. Line 14 will also log 150. the var finalPrice also gets last modified during the last iteration of the loop. we rounded 15000 and then divided by 100
4. [ 50, 100, 150 ]. the function returns discounted, which is an array. every iteration of the for loop we calculate the finalPrice for each of the original prices and push it to the discounted array.
5. line 12 will throw an error. i will not be defined by the time we access it. We used `let` to assing i, and the scope of it would be the for loop. we then referred to i at line 12, which is out of scope
6. line 13 will throw an error. discountedPrice could not be found when we call it. this is because we used `let` to assing discountedPrice, so the scope of it would be within the for loop. As such, line 13 would be out of scope.
7. line 14 will return 150. finalPrice is defined in line 4 within the function, which means that the finalPrice is defined within the scope of the function. line 14 would 
8. The function will return [ 50, 100, 150 ]. the function returns discounted, which is an array defined with `let`, which is valid within the function. every iteration of the for loop we calculate the finalPrice for each of the original prices and push it to the discounted array.
9. line 11 will throw an error. Similar to above, i is defined with `let`, which means that it will not be valid outside of the for loop scope
10. line 12 will print 3 because length is defined in line 4 as the length of prices. it is defined with `const` so it is valid within the function scope.
11. the function returns [ 50, 100, 150 ]. Even though the `discounted` array is defined with `const`, we can still manipulate the array. We just can't reassign it. So the function will work as intended
12. q12
    1.  A - student.name
    2.  B - student['Grad Year']
    3.  C - student.greeting()
    4.  D - student['Favorite Teacher'].name
    5.  E - student.courseLoad[0]
13. 
    1.  A - '32' : intergers map to ther exact string representaion and we are concatenating
    2.  B - 1 :'3' got comverted to the integer 3. then we subtract 2
    3.  C - 3 : null got converted to 0
    4.  D - '3null' : null got converted to 'null', then concatenated
    5.  E - 4 : true got converted to 1 then added to 3
    6.  F - 0 : false converted to 0. null converted to 0
    7.  G - '3undefined' : 3 undefined got converted to 'undefined' then concatenated
    8.  H - NaN : we can't convert undefined to an integer so it will be undefined
14. 
    1.  A - true. '2' becomes integer 2
    2.  B - false. '2' string is bigger than '12' because it started with 2
    3.  C - true. '2' becomes integer 2
    4.  D - false, '2' and 2 are two different types
    5.  E - false, true gets converted to 1
    6.  F - true, Boolean(2) gets converted to true
15. The `==` operator checks for equality after converting both operands to a common type while the `===` operator, also known as the strict equality operator, checks for equality without performing type conversion.
16. done with js file
17. the function will return [2,4,6]. modifyArray iterates through `array` and applies callback to each element of array and append it to new array. in this case, our function multiplies the element by 2. so we should get an array back that times each element by 2.
18. done with js file
19. the out put is
1
4
3
2
we log 1 first. then 2 is logged 1 second after. then 3 is logged immediately after all the other immediately executed codes (log 4).