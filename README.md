# Simple Calculator

This is a simple calculator web application designed and developed by [AR7](https://ar123456.netlify.app/). It includes basic arithmetic operations and a user-friendly interface.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)

## Demo

You can see the live demo of the calculator [here](https://webcalculator-ar7.netlify.app/).

## Features

- Addition, Subtraction, Multiplication, and Division operations
- Clear (AC) and Delete (DE) functions
- Decimal point input
- Responsive design

## Installation

To use this calculator locally, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/ThisIsAR7/Web-Calculator.git
    ```
2. Navigate to the project directory:
    ```sh
    cd Web-Calculator-main
    ```

## Usage

Open the `index.html` file in your preferred web browser to use the calculator.

### Calculator Structure

- **HTML**: The structure of the calculator
- **CSS**: Styling for the calculator, located in `css/style.css`
- **JavaScript**: Inline JavaScript for basic functionality

### Example

The calculator includes buttons for numbers, operators, and control actions (AC and DE). Click on the buttons to perform calculations.

```html
<div class="calculator">
    <form>
        <div class="display">
            <input type="text" name="display">
        </div>
        <div>
            <input type="button" value="AC" onclick="display.value = '' " class="operator">
            <input type="button" value="DE" onclick="display.value = display.value.toString().slice(0,-1)" class="operator">
            <input type="button" value="." onclick="display.value += '.' " class="operator">
            <input type="button" value="/" onclick="display.value += '/' " class="operator">
        </div>
        <div>
            <input type="button" value="9" onclick="display.value += '9' ">
            <input type="button" value="8" onclick="display.value += '8' ">
            <input type="button" value="7" onclick="display.value += '7' ">
            <input type="button" value="*" onclick="display.value += '*' " class="operator">
        </div>
        <div>
            <input type="button" value="6" onclick="display.value += '6' ">
            <input type="button" value="5" onclick="display.value += '5' ">
            <input type="button" value="4" onclick="display.value += '4' ">
            <input type="button" value="-" onclick="display.value += '-' " class="operator">
        </div>
        <div>
            <input type="button" value="3" onclick="display.value += '3' ">
            <input type="button" value="2" onclick="display.value += '2' ">
            <input type="button" value="1" onclick="display.value += '1' ">
            <input type="button" value="+" onclick="display.value += '+' " class="operator">
        </div>
        <div>
            <input type="button" value="000" onclick="display.value += '000' ">
            <input type="button" value="0" onclick="display.value += '0' ">
            <input type="button" value="00" onclick="display.value += '00' ">
            <input type="button" value="=" onclick="display.value = eval(display.value)" class="operator">
        </div>
    </form>
</div>
