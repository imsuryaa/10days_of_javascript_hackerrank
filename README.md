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

- `let` and `const`, Print the area and perimeter of circle

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

## Day 2
- Create a `getGrade()` function to validate the grade based on the score
- Constraints: `0 <= score <= 30`

```
function getGrade(score) {
    let grade;
    if(score<=30) grade = "A"
    if(score<=25) grade = "B"
    if(score<=20) grade = "C"
    if(score<=15) grade = "D"
    if(score<=10) grade = "E"
    if(score<=5) grade = "F"
    return grade;
}
```

- Conditional Statements: Switch

```
function getLetter(s) {
    let letter;
    switch(s[0]){
        case ('a' || 'e' || 'o' || 'i' || 'u'):
            letter = "A"
            break
        case ('b' || 'c' || 'd' || 'f' || 'g'):
            letter = "B"
            break
        case ('h' || 'j' || 'k' || 'l' || 'm'):
            letter = "C"
            break
        case ('z' || 'n' || 'p' || 'q' || 'r' || 's' || 't' || 'v' || 'w' || 'x' || 'y'):
            letter = "D"
            break
        
    }
    return letter;
}
```

- `Loops`: Print vowels and consonants on each line from the given string.
- First print vowels and second print consonants

```
let vowels = "aeiou"
let consonants = ""
function vowelsAndConsonants(s) {    
    for(let l of s){
        vowels.includes(l) ? console.log(l) : consonants += l + "\n"
    }
    console.log(consonants)
}
```
