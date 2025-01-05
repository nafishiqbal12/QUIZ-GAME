# Quiz Game in C

## Overview
This project is a simple **Quiz Game** implemented in C. The game presents a set of multiple-choice questions to the player, who must select the correct answer to score points. The questions are chosen randomly to make the game more engaging.

---

## Features
- **Randomized Questions**: Questions are picked randomly from a predefined set.
- **Multiple-Choice Options**: Each question has four options to choose from.
- **Score Tracking**: The player’s score is calculated based on correct answers.

---

## Implementation Details

### Data Structure
The `Question` structure is used to store the following details for each question:
- `question`: The quiz question as a string.
- `options[4]`: An array containing four possible answers.
- `correct_options`: An integer representing the correct option (1-based index).

### Core Functions
1. **`displayQuestion(Question q)`**
   - Displays a question and its corresponding options.

2. **`checkAnswer(Question q, int user_answer)`**
   - Checks if the user's selected option matches the correct answer.

### Game Flow
1. The program initializes a list of predefined questions.
2. Questions are randomized using `rand()`.
3. For each question:
   - The question and its options are displayed.
   - The user selects an option.
   - The user's answer is validated, and the score is updated.

---

## How to Run the Program
1. **Compile the Program**
   Use a C compiler to compile the program:
   ```bash
   gcc -o quiz_game quiz_game.c
   ```

2. **Run the Program**
   Execute the compiled program:
   ```bash
   ./quiz_game
   ```

3. **Follow the Instructions**
   Answer the questions as they appear to complete the quiz.

---

## Example Questions
- **Question**: "Which bird lays the largest egg?"
  - Options:
    1. Owl
    2. Ostrich
    3. Kingfisher
    4. Woodpecker
  - Correct Answer: 2 (Ostrich)

- **Question**: "How many legs does a spider have?"
  - Options:
    1. 7
    2. 8
    3. 11
    4. 4
  - Correct Answer: 2 (8)

---

## Known Issues
- **Incomplete Game Logic**: The program does not currently prompt the user for their answer or update the score.
- **Uninitialized Variables**: Variables such as `current_questions` are referenced but not properly declared or used.

---

## Future Enhancements
- Add input handling to allow users to answer questions.
- Display the final score at the end of the quiz.
- Include more questions to make the game more diverse.
- Implement a timer for each question to increase the challenge.

---

Enjoy playing the Quiz Game! 🎉

