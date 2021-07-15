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
