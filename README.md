# test.cc

## Code modification
This repository contains a rice cooker simulation with features for adding rice, cooking rice, steaming rice, keeping rice warm, and removing rice from the cooker.

## Changes made
The original code was based on if/else if statements to handle user choices. Here are the main changes made:

### 1.Integration of the switch case structure: 
if/else if statements have been replaced by a switch case structure. This makes the code easier to read and more efficient in managing the various user options.

### 2.Refactoring for the use of modules: 
Imports and exports have been configured to use ES6 modules, enabling better code structuring.

### 3.Potential bugs fixed: 
The menu.js file is imported to display the menu, and minor adjustments have been made to ensure that functions are correctly called.
N.B: you'll also need Ny Ando Mayah's "menu.js
## Code usage
The main file is main.js. To run it, make sure you have Node.js installed. Use the node main.js command in your terminal to start the rice cooker simulation. Follow the instructions displayed to interact with the simulator.

## Note
Be sure to install the necessary dependencies by running npm install to obtain the required packages, including prompt-sync for user input management.
N.B: you'll also need Ny Ando Mayah's "menu.js

## Functions and Complexity

    - The codebase primarily involves constant time operations within the riceCooker methods. Operations like adding rice, cooking, and keeping warm have constant complexity regardless of input size. The simulateRiceCooker() function contains a while loop with linear complexity based on the number of iterations required to complete the program.

## Complexity Tool
    - To analyze the complexity more precisely, I used Big O Calculator to estimate the overall complexity of the code.

### 1. `addRice()`: O(1)
    - The time complexity of this function is O(1) because it only performs a constant number of operations, regardless of the size of the input. The function checks if the "ricePresent" property is true or false, updates the property, and prints a message to the console.

    - The space complexity of this function is O(1) because it does not use any additional data structures that grow with the size of the input. It only updates the "ricePresent" property and prints a message to the console, which do not require additional memory allocation.

### 2. `cookRice()`: O(1)
    - The time complexity of the cookRice() function is O(1) because it has a constant number of operations that do not depend on the size of the input. The function checks the values of two boolean variables and performs a few console.log statements, which all take constant time.

    - The space complexity of the cookRice() function is O(1) because it does not use any additional space that grows with the size of the input. The function only uses a few boolean variables and does not create any new data structures or variables.

### 3. `steam()`: O(1)
    - Initiates steaming if rice is present and not already steaming. Introduces a delay of 1500ms.
    The time complexity of this steam() function is O(1) because the execution time does not depend on the input size. It always performs a constant number of operations, regardless of the state of the rice cooker.

    - The space complexity of this function is also O(1) because it does not use any additional data structures that grow with the input size. It only uses a few boolean variables to keep track of the state of the rice cooker.

### 4. `keepWarm()`: O(1)
    - The time complexity of this function is O(1) because the execution time is constant regardless of the input size. The function only performs a few simple conditional checks and prints a message.

    - The space complexity of this function is also O(1) because it does not use any additional data structures that grow with the input size. It only uses a few boolean variables to track the state of the rice cooker.

### 5. `removeRice()`: O(1)
    - The time complexity of this function is O(1) because it only performs a constant number of operations regardless of the size of the input. The space complexity is also O(1) because it does not use any additional memory that scales with the input size.

### 6. `delaySync(ms)`: O(n) (where 'n' is the value of 'ms')
    - The time complexity of this function is O(ms) because the while loop will run for a duration of "ms" milliseconds. The space complexity is O(1) because no additional space is used in the function.

### 7. `simulateRiceCooker()`: Variable
    - The time complexity of this function is O(n), where n is the number of iterations in the while loop. This is because the function will continue to run as long as the condition is true, and the number of iterations depends on the user's input and choices.

    -The space complexity of this function is O(1), as it only uses a constant amount of memory for the input variable and the condition variable. The function does not create any additional data structures or variables that depend on the input size.


