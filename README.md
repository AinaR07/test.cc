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

The codebase primarily involves constant time operations within the riceCooker methods. Operations like adding rice, cooking, and keeping warm have constant complexity regardless of input size. The simulateRiceCooker() function contains a while loop with linear complexity based on the number of iterations required to complete the program.

### Complexity Analysis

### 1. `addRice()`: O(1)
- **Time Complexity**: The function performs a constant number of operations, independent of input size, to check and update the "ricePresent" property and print a message to the console.
- **Space Complexity**: Requires constant memory as it updates a property and performs console output without additional data structures.

### 2. `cookRice()`: O(1)
- **Time Complexity**: Performs constant operations checking boolean variables and console outputs, independent of input size.
- **Space Complexity**: Requires constant memory, uses a few boolean variables without new data structures.

### 3. `steam()`: O(1)
- **Time Complexity**: Constant operations regardless of input size, initiates steaming with a fixed delay.
- **Space Complexity**: Utilizes a few boolean variables, doesn't create data structures scaling with input.

### 4. `keepWarm()`: O(1)
- **Time Complexity**: Executes a few simple conditional checks and prints a message, regardless of input size.
- **Space Complexity**: Uses boolean variables without additional data structures, constant memory.

### 5. `removeRice()`: O(1)
- **Time Complexity**: Constant operations regardless of input size, updates properties.
- **Space Complexity**: Requires constant memory, no additional memory allocation.

### 6. `delaySync(ms)`: O(n) (where 'n' is the value of 'ms')
- **Time Complexity**: Runs a while loop for 'ms' milliseconds, linear time based on 'ms'.
- **Space Complexity**: No additional space used, constant memory.

### 7. `simulateRiceCooker()`: Variable
- **Time Complexity**: Linear complexity based on the number of iterations in the while loop, dependent on user input and choices.
- **Space Complexity**: Constant memory usage, no additional data structures created.
