# 10days_of_javascript_hackerrank

## Day 1

- Calculate the area and perimeter of rectangle

```
function getArea(length, width) {
    let area;
    area = length * width;
    return area;
}
function getPerimeter(length, width) {
    let perimeter;
    perimeter = 2 * (length + width);
    return perimeter;
}
```

- Implement a function which gives a factorial of a number

```
function factorial(n){
    let num = 1
    for(let i=1; i<=n; i++){
        num *= i
    }
    return num
}
```

- Let and Const, Print the area ans perimeter of circle

```
function main() {
    // Write your code here. Read input using 'readLine()' and print output using 'console.log()'.
    let r = parseFloat(readLine())
    const PI = Math.PI
    // Print the area of the circle:
    console.log(PI*r*r)
    // Print the perimeter of the circle:
    console.log(2*PI*r)
    try {    
        // Attempt to redefine the value of constant variable PI
        PI = 0;
        // Attempt to print the value of PI
        console.log(PI);
    } catch(error) {
        console.error("You correctly declared 'PI' as a constant.");
    }
}
```
