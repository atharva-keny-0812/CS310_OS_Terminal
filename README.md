# Custom Linux Shell: Hogwarts Terminal

Welcome to the **Hogwarts Terminal**, a custom Linux shell inspired by the four Hogwarts houses: Gryffindor, Slytherin, Hufflepuff, and Ravenclaw. Each house offers unique commands and functionalities to enrich your shell experience. 



## Features

- **Interactive shell**: Execute Linux commands, including piped commands.
- **House-specific commands**:
  - **Gryffindor**: Focused on file organization and cleanup.
  - **Slytherin**: File manipulation and hidden directory operations.
  - **Hufflepuff**: File management best practices and encouragement.
  - **Ravenclaw**: Wisdom quotes, riddles, and file search utilities.
- **Custom greeting and Sorting Hat ceremony** to select your house.
- Integrated help system for custom commands.



## How to Use

1. **Compile the Code**:  
   Use the GCC compiler to build the program:
   ```bash
   gcc -o house_shell house_shell.c -lreadline

2. **Run the Shell**:  
  Launch the shell using:
  bash
  ./house_shell  
  

3. **Sorting Hat Ceremony**:
Answer the questions to be sorted into a house.

4. **Explore Your House Commands**:
Use the terminal to execute house-specific commands or general Linux commands. Type help to get a list of available commands.

### House-Specific Commands  
- **Gryffindor Terminal**  
   - expelliarmus: Delete corrupted files.  
  - protego: Backup good files.  
  - homenumRevelio: Move hidden files to the main directory.  
- **Slytherin Terminal**  
  - imperius: Clear file contents or modify files.  
  - serpensortia: Generate corrupted files.  
  - obscuro: Hide files in a hidden directory.  
- **Hufflepuff Terminal**  
  - amortentia: Creates new text files.  
  - patronus: Provide encouraging messages.  
  - prudens: Display file management best practices.  
- **Ravenclaw Terminal**  
  - ravenfacts: Display a random wisdom quote.  
  - quizme: Challenge yourself with a riddle.  
  - findHorcrux: Search for a file named horcrux.txt.  

### General Commands  
- **help [command]**: Display detailed information about a specific command.  
- **exit**: Exit the shell.  

Code Structure
---------------------------------------------------------------
init_shell(): Displays the welcome message and clears the screen.  
takeInput(): Captures user input.  
execArgs(): Executes simple commands.  
execArgsPiped(): Executes piped commands.  
processString(): Parses input and determines execution type.  
shell_cmds(): Runs the main shell loop for a specific house.  
sortingHat(): Sorts the user into a house.  
Pipes: The shell supports pipes, enabling users to chain commands.  
Themed Shell: The shell is themed around the four Hogwarts houses, with specific commands unique to each house.  
Command Execution: External commands and house-specific commands are executed using execvp in child processes created by fork.  
Interactive User Experience: The program interacts with the user, providing help and sorting them into a "house" based on their preferences.

Dependencies
---------------------------------------------------------
Linux environment
readline library for interactive input.

Contributing
--------------------------------------------------------------
Feel free to fork this repository and add your own custom commands or features. Pull requests are welcome!



Acknowledgments
-----------------------------------------------------------------------
Inspired by the Harry Potter series for house-based customization.
Designed for educational and recreational purposes.