1. It prints the value of prices.length because it is declared with 'var', which is globally/function scoped. It's not local to the loop.

2. It prints the last value it is assigned of "prices[i] * (1 - discount)", where i = prices.length - 1. This is also because var is globally scoped, despite being assigned multiple times in the loop.

3. It prints the final value of discountedPrice but rounded to 2 decimal places, as it is reassigned inside the loop.

4. It returns the array of the discounted price of each item, [50, 100, 150], as each price is appended to the list after applying the discount value.

5. An error is returned because i is defined with 'let', so it's not accessible outside the loop.

6. An error is again returned because discountedPrice is only defined within the loop.

7. It prints the final value discountedPrice is assigned to, but rounded to 2 decimal places. This is because discountedPrice is declared outside the loop, so its value can be reassigned or accessed anywhere in the function.

8. It returns an error due to trying to access an uninitialized variable. If we disregard this error, it would return the array [50, 100, 150], for identical reasons as before.

9. An error is returned, as i is inaccessible outside of the loop due to being defined with "let".

10. An error is returned because 'const' is scoped. discountedPrice is only accessible within the loop.

11. The command should print "0", as finalPrice is a constant, meaning its initial declaration value is always its value. This is of course ignoring the errors that would've been thrown when a constant was reassigned.

12. It should return [50, 100, 150]. This is because the constant 'discounted' still points to the same list, we're just adding to that list.

13. 
a) student.name
b) student["Grad Year"]
c) student.greeting()
d) student["Favorite Teacher"].name
e) student.courseLoad[0]

14. 
a) '32', because '3' is a string and it's first so '2' is converted to a string as well and then concatenated.
b) 1; '3' is converted to a number type because subtraction can't be applied to strings.
c) 3; the first type is a number, so null is treated as 0.
d) '3null', as null is converted to a string.
e) 4, as true is treated as 1 when adding numbers.
f) 0, because both false and null are treated as 0 when converted to numbers during addition.
g) '3undefined'. "3" is a string so undefined is converted to a string and concatenated.
h) NaN, because subtraction means a number based operation, but undefined cannot be converted to a number, so subtraction results in NaN, or Not a Number.

15. 
a) true, as JS converts values to numbers when 2 different types are being compared.
b) false; lexicographically, '2' is greater, as '2' is the first character and greater than '1'.
c) true, as JS converts the string '2' to a number.
d) false, as '===' compares without conversion, and a number is not the same as a string.
e) false, as true is converted to 1, which is not equal to 2.
f) true, because Boolean(2) returns true (Boolean() returns true whenever the parameter is not in a set of values such as 0, NaN, etc).

16. == checks equality but performs type conversion if necessary, while === does not perform any type conversion.

17. 'How are you' is printed, as in the first comparison, true is converted to 1 which is not equal to 2. As stated earlier, Boolean(2) returns true so if(2) evalutes to true.

18. In corresponding js file

19. The function returns [6, 8, 10]. This is because for each element in the array it operates it on it by calling doSomething, which calls function(x). The result is (num + 2) * 2, which is then appended to newArr.

20. In corresponding js file

21. The function prints 1, 4, 3, 2 on separate lines.