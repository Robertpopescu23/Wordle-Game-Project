# Wordle Game

A single-player Wordle game built using HTML, CSS, and JavaScript. Players guess a five-letter word within six attempts. The game provides feedback for each guess, indicating correct, present, or absent letters.

---

## Features

- **Single-player Wordle Challenge:** Guess the target word in six attempts.
- **Feedback Mechanism:**  
  - **Correct Letter & Position:** Green cell with white text.  
  - **Letter Present but Wrong Position:** Yellow cell with black text.  
  - **Letter Not in Word:** Gray cell with white text.
- **Random Word Selection:** Game selects a random word from a list of 600 words.
- **Responsive Design:** Centered text, clean layout, and styled buttons for better user experience.
- **Game Over Conditions:**  
  - Correct guess: Displays a success message.  
  - Exhausted attempts: Displays the correct word and ends the game.

---

## Technologies Used

- HTML (DOM Selection & Manipulation)
- CSS (Styling & Layout)
- JavaScript (Conditionals, Functions, Event Handling)

---

## Game Layout & Styling

- **Heading:** Wordle Game displayed at the top.
- **Input Field:** Accepts up to 5 letters, auto-focused when the game starts.
- **Submit Button:** Bold, padded, centered below the game board.
- **Game Board:**  
  - Grid layout with 5 cells per row.  
  - Each cell is a square with spacing between cells.  
  - White background, slight border, rounded corners.  
- **Feedback Message:** Bold, easy to read, displayed below the submit button.  

**Example Placeholder Message:**  
`Congratulations! You guessed the word!`

---

## Game Logic

1. **Initialize Game:**
   - Load an array of 600 words.
   - Select a random word as the target word.
2. **User Guess Submission:**
   - Check if the input is exactly 5 letters.
   - Compare each letter with the target word:
     - Correct position → Green cell.
     - Present but wrong position → Yellow cell.
     - Absent → Gray cell.
3. **Update Game State:**
   - Display feedback message after each guess.
   - Disable input if the word is guessed correctly or all attempts are used.
4. **Game End:**
   - If guessed correctly → Show success message.  
   - If attempts exhausted → Show game-over message with the correct word.

---

## Instructions

1. Open `index.html` in a web browser.
2. Type a 5-letter word in the input field.
3. Click **Submit Guess** or press **Enter**.
4. Observe feedback on the game board.
5. Continue until you guess the word or use all 6 attempts.

---

## Notes

- The game uses a predefined list of 600 words (provided in the project resources).
