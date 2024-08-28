This Python script implements a simple Rock-Paper-Scissors game with a graphical user interface (GUI) using the Tkinter library. The game allows a user to play against the computer, with both scores being tracked. Here is a detailed description of the code:

1. Importing Libraries:
tkinter: The Tkinter library is used to create the GUI components.
random: The random module is used to allow the computer to make a random choice between Rock, Paper, and Scissors.
2. Game Logic - determine_winner(user_choice):
Options: The available choices for the game (Rock, Paper, Scissors) are stored in a list.
Computer Choice: The computer randomly selects one of the options using random.choice(options).
Result Calculation:
If the user’s choice is the same as the computer’s, it’s a tie.
If the user’s choice beats the computer’s choice (based on Rock-Paper-Scissors rules), the user wins and their score is incremented.
Otherwise, the computer wins and its score is incremented.
UI Updates: The labels displaying the results, user choice, computer choice, and scores are updated based on the outcome.
3. Resetting the Game - reset_game():
This function resets the scores (user and computer) to zero.
It also clears the result and choice labels to prepare for a new game.
4. Exiting the Game - exit_game():
This function closes the application by calling root.quit().
5. Creating the Main Window:
root = tk.Tk(): Initializes the main application window.
root.title("Rock Paper Scissors"): Sets the window title to "Rock Paper Scissors".
root.geometry("400x600"): Specifies the size of the window.
root.configure(bg="#F0F0F0"): Configures the background color of the window to a light gray.
6. UI Components:
Header and Sub-header Labels:
Display the game title and a brief subtitle.
Score Label:
Displays the current score between the user and the computer, initially set to 0 - 0.
Choice Labels:
Display the user’s choice and the computer’s choice after each round.
Result Label:
Displays the result of each round, such as "You Win!" or "You Lose!".
Buttons for User Choices:
Three buttons ("Rock", "Paper", "Scissors") allow the user to make their choice. When clicked, they call determine_winner() with the corresponding choice as the argument.
Reset Button:
Resets the game by calling reset_game(), clearing scores and results.
Button Layout:
The buttons are organized in a grid layout inside a frame, with some padding for spacing.
7. Running the Application:
root.mainloop(): Starts the Tkinter event loop, making the application responsive and interactive.
8. User Interaction:
Playing the Game:
The user selects "Rock," "Paper," or "Scissors" by clicking the respective button.
The computer randomly selects one of the options, and the result of the round is displayed, including the choices and updated scores.
Resetting the Game:
The user can reset the game at any time by clicking the "Reset" button, which clears all data.
Exiting the Game:
The application can be closed by clicking the "Exit" button (though this functionality is not directly included in the script provided but could be added easily).
Dependencies:
Tkinter: The script relies on Tkinter for the graphical interface, which is usually included with Python.
random: Part of Python's standard library, no additional installation is required.
