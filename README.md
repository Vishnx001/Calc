# Ex.08 Design of a Standard Calculator
## Date: 23-04-2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
calc.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" type="text/css" href="calc.css">
</head>
<body>
<h1>ABISHAI 212223240002</h1>
<div class="calculator">
    <input type="text" id="display" readonly>
    <input type="button" value="7" onclick="addToDisplay('7')">
    <input type="button" value="8" onclick="addToDisplay('8')">
    <input type="button" value="9" onclick="addToDisplay('9')">
    <input type="button" value="/" onclick="addToDisplay('/')">
    <input type="button" value="4" onclick="addToDisplay('4')">
    <input type="button" value="5" onclick="addToDisplay('5')">
    <input type="button" value="6" onclick="addToDisplay('6')">
    <input type="button" value="*" onclick="addToDisplay('*')">
    <input type="button" value="1" onclick="addToDisplay('1')">
    <input type="button" value="2" onclick="addToDisplay('2')">
    <input type="button" value="3" onclick="addToDisplay('3')">
    <input type="button" value="-" onclick="addToDisplay('-')">
    <input type="button" value="0" onclick="addToDisplay('0')">
    <input type="button" value="." onclick="addToDisplay('.')">
    <input type="button" value="=" onclick="calculate()">
    <input type="button" value="+" onclick="addToDisplay('+')">
    <input type="button" value="C" onclick="clearDisplay()">
</div>

<script src="calc.js"></script>

</body>
</html>

```
```
calc.css

.calculator {
    width: 220px;
    margin: 0 auto;
    border: none;
    border-radius: 15px;
    padding: 10px;
    background-color: #fe0404;
    display: grid;
    grid-template-columns: repeat(4, 50px);
    grid-gap: 5px;
}

input[type="button"] {
    width: 50px;
    padding: 10px;
    font-size: 18px;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    background-color: #646867;
    color: white;
}

input[type="text"] {
    grid-column: span 4;
    padding: 10px;
    font-size: 18px;
    border: 1px solid #0b0b0b;
    border-radius: 15px;
}

```

```
calc.js
function addToDisplay(value) {
    document.getElementById('display').value += value;
}

function calculate() {
    var expression = document.getElementById('display').value;
    var result = eval(expression);
    document.getElementById('display').value = result;
}

function clearDisplay() {
    document.getElementById('display').value = '';
}
```
## OUTPUT:

![Screenshot (20)](https://github.com/Abishai95141/Calc/assets/139335314/84c93bb1-5657-4c29-a0b2-748d8963f58e)


![Screenshot (21)](https://github.com/Abishai95141/Calc/assets/139335314/8d39c1c2-cc0a-4522-9928-d86436ac4e48)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.

