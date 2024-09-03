# Dice Roller Project
- This Java application processes dice roll expressions from an input file and outputs the results as a JSON file.
- It supports standard polyhedral dice with various sides (e.g., d4, d6, d8, d10, d12, d20) and allows combinations of dice rolls, addition, subtraction, and integer modifiers.


  # Table Of Contents
 * 1. Features
 * 2. Languages
 * 3. Project Structure
 * 4. Usage
 * 5. Input Format
 * 6. Output Format
 * 7. How To Run Application
 * 8. Troubleshooting
 * 10. Contact


 # Features
- Dice Roll Evaluation: Supports expressions like 2d6 + d8 + 4 or D20 - 1 + 4d12.
- JSON Output: Outputs results with the calculated roll, minimum possible result, and maximum possible result
      

 # Languages: 
 - Java
  
# Project Structure
dice-roller/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── diceroller/
│   │   │               ├── DiceRoller.java
│   │   │               └── DiceRollerParse.java
|   |   |               └── DiceRollerResult.java
│   │   └── resources/
│   └── test/
│       ├── java/
│       └── resources/
├── input.txt              # Place your input.txt file here
├── output.json            # Output file (if specified)
├── pom.xml
└── README.md

# Usage

 * Run the program by providing the input file as the first argument.
 * Optionally, specify an output file as the second argument.
 * java -jar target/dice-roll-parser.jar input.txt 
 * Optionally, specify an output file:
 * java -jar target/dice-roll-parser.jar input.txt output.json

# Input Formate
- input.txt
- (pass input value like that
-  2d6 + d8 + 4
  D20 - 1 + 4d12
)
# Output Formate
-  output.json
-  Output will get like that: {"rollResult":25,
-  "rollMin":17,
-  "rollMax":47}
  

# How to Run the Application
# Prerequisites
- Java 8 or higher
- Maven
- IntelliJ IDEA (or any other IDE)

# Place the Input File:

- Create an input.txt file in the root directory of the project.
- Add your dice roll expressions, one per line.
- Open in IntelliJ IDEA:

# Open IntelliJ IDEA.
- Select "Open" and choose the dice-roller directory.
- Allow IntelliJ to import the Maven project.
  
# Configure Run/Debug Configurations:
- Go to "Run" > "Edit Configurations...".
- Click "+" to add a new "Application" configuration.
  
# Set the following:
 - Name: DiceRoller
- Main class: com.example.dice.DiceRoller
- Program Arguments: input.txt output.json
- Working Directory: Set to your project root (where input.txt is located).
  
# Run the Application:

- Select the DiceRoller configuration.
- Click the green "Run" button.

# Troubleshooting
- Ensure the paths are correct: Verify that input.txt is in the correct directory and specified correctly in program arguments.
- Check file permissions: Make sure the application has read access to input.txt and write access to output.json .

# Contact
- Contact: 9696481593
- Gmail: abhishek184april.gmail.com
- LinkedIn: https://www.linkedin.com/in/abhishek-singh-38b2bb1b9
