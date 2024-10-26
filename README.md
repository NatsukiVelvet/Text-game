LEGEND OF IOKA 
## PROJECT OVERVIEW

- Legend of Ioka is a turn-based role-playing game (RPG) where players step into the shoes of Nikolas and   Eli, descendants of legendary heroes Killain and Landon. Together, they must prevent the resurgence of the Order of the Midnight Sun- a group of terrorists that plan to destroy Ioka. 


- Legend of Ioka solves the problem of offering an engaging, story-driven RPG experience by combining immersive storytelling, strategic turn-based combat, and exploration within a rich world filled with lore, danger, and adventure. Built in Java, it provides players with meaningful character development and tactical decision-making in battles, all in a lightweight, text-based format that is accessible in coding environments, making it ideal for those who prefer or are limited to non-graphical interfaces.

## HOW TO RUN THE PROGRAM
1. Unzip the folder majorAssignmentTopic1
2. Open VScode
3. “Open Folder…” in Vscode
4. Select the folder majorAssignmentTopic1
5. Open the file Main.java
6. Run the program

PROJECT STRUCTURE
/Story_folder
 ├── Intro.txt 
 ├── ActOne.txt 
 ├── ActTwo.txt 
 ├── ActTwo_2.txt 
 ├── ActTwo_3.txt 
 ├── ActTwo_final.txt 
 ├── ActThree.txt 
 ├── ActThree_2.txt   
 ├── Thanks.txt 

/Java Classes
  ├── Character.java 
  ├── Item.java 
  ├── Main.java 
  ├── Move.java 
  ├── Player.java 
  ├── GameLogic.java 
  ├── testingJUnit.java 
More information in BUILDING CLASS STEPS below



## ALGORITHMS AND LOGIC

Most important algorithms, algorithm of lesser importance will be documented in detail in Document.docx

# ** Read Integer Input Algorithm **
- Reads input from the user
-  Ensures input are acceptable by comparing against the allowed input range 
- In case user entered a String, will catch the error and read a warning telling user to enter Integer

# **Game loop/ Battle loop Algorithm:**
- Loops to continue playing the game
- Checking for a boolean variable for the game’s state, either running or not .
- Reads input and calls corresponding methods to advance in the game

# **Story Display:**
- Handles the display of Story text, ensuring the advancement of gameplay.


## FUNCTIONAL REQUIREMENTS
# 1. Character Management
- Players can interact with and manage their characters' attributes such as Attack (ATK), Magic, Health Points (HP), Defense (DEF), Magic Defense (Mag_DEF), and Speed through a menu-based system in the command-line interface.

- Each character can equip an unlimited number of items, which dynamically alter their stats, enhancing their abilities in battle. Items may boost or reduce specific attributes (e.g., ATK, DEF, Magic) depending on the item equipped.

# 2. Battle Mechanics
- Battles are turn-based, where the action gauge determines when a character can act.
- Players choose actions such as attacking, using magic, healing, or summoning.
- Characters can critically hit, which amplifies damage based on their critical chance stat.

# 3. Story Progression
- The game follows a detailed storyline with three acts:
    + Act 1: Unheard Cries
    + Act 2: Unquelled Anger
    + Act 3: Unfinished Writing (Dev note: I was tired to edit the story)

# 4. Item System
- Items boost character stats such as ATK, DEF, Magic, etc.
- Items can be equipped, unequipped, and their effects are dynamically applied before battles.

# 5. Scoring system
- Once players finish the game or perish during battle, their final score is loaded into result.csv


## NON-FUNCTIONAL REQUIREMENTS
# 1. Persistence and Compatibility
    - Score Display and Export:
        + At the end of the game, players' final scores are exported to CSV format, ensuring compatibility with applications like Microsoft Excel and Google Sheets.

    - File Accessibility:
        + The exported CSV file containing the score is easily accessible and transferable, allowing players to save or share their results for future reference.
# 2. Performance and Scalability
    - Efficient Game Logic:
        + The game efficiently handles battle mechanics, story progression, and item management with minimal latency, ensuring a smooth player experience.

    - Resource Management:
        + The game is optimized for development environments like VSCode, requiring players to have Java SE 11 or higher to compile and run the game. While it can run on systems with moderate resources, players need a Java development environment to run the game.

# 3. Flexibility and Maintainability
    - Modular Code Structure:
        + The application is designed with a modular structure, allowing for easy updates and the addition of new features like new characters, items, or storylines.
    - Customizability:
        + While the codebase allows developers to add new moves, characters, or subplots, it may influence the story or gameplay experience, necessitating changes to the storyline or battle sequence.

# 4. Error Handling and Validation
    - Input Validation:
        + The system checks for valid input values during combat (e.g., choosing valid targets, ensuring correct inputs during menu navigation).
    - Combat and Story Conflicts:
        + The game quietly waits for correct inputs, allowing only valid moves or choices, ensuring smooth gameplay without the need for error messages or alerts.


# 5. Documentation and Usability
    - Comprehensive Documentation:
        + The project includes detailed user and developer documentation, explaining game setup, battle mechanics, item usage, and code structure for developers.
    - User-Friendly Interface:
        + Although the game operates via a command-line interface, interactions are clear and intuitive for players to navigate, with simple prompts and feedback throughout the game.



## FUTURE ENHANCEMENTS
- Further improve the input system to alert the user of “out of bounds” numerical input as well, not just String input
- Improvements to CLI (command line interface) and how the text is displayed
- Expand the storyline with more acts and character development.
- Save state for the game


