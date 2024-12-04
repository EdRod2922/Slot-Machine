# Slot-Machine

Overview

This Python program simulates a simple slot machine game where users can deposit money, place bets, and spin the reels to try their luck. It features realistic mechanics like betting across multiple lines, configurable symbol probabilities, and winnings calculations based on symbol values. The program leverages advanced logic and Python syntax to ensure functionality, modularity, and an engaging user experience.
Features

    Deposit System
    Users can deposit money to play the game. Input validation ensures that only positive numerical amounts are accepted.

    Configurable Betting
        Users select the number of lines to bet on (up to a maximum limit).
        Bets per line are validated to fall within a specified range, ensuring players cannot bet more than their balance.

    Slot Machine Logic
        Symbols and their probabilities are defined in a dictionary, ensuring a fair and adjustable game experience.
        A spinning function simulates the random selection of symbols for the slot machine reels.

    Winnings Calculation
        Winning lines are determined based on matching symbols across the selected lines.
        The program calculates payouts based on predefined symbol values and the player's bet amount.

    Interactive User Experience
        Results are displayed in a readable grid format.
        Users receive feedback on their winnings and have the option to continue playing or quit.

Thought Process and Advanced Logic
Modularity and Function Design

    The program is broken into distinct functions, each handling a specific aspect of the game:
        deposit(), get_number_of_lines(), and get_bet() handle user input.
        get_slot_machine_spin() generates the slot machine's reels.
        check_winnings() determines winnings based on game rules.
        spin() manages the core gameplay loop.
        main() provides a cohesive structure for the game, ensuring a smooth user flow.

Symbol Management

    Symbol Probability: Symbols are added to a list multiple times based on their respective probabilities (e.g., "A" appears twice, while "D" appears eight times). This allows for dynamic control over the likelihood of specific outcomes.
    Random Selection: The use of random.choice ensures fair randomness while removing selected symbols to avoid duplication.

Winning Line Logic

    Nested loops and advanced conditional checks are used to verify whether all symbols in a line match.
    The else clause on the for loop is a subtle yet powerful way to handle scenarios where all symbols on a line match without needing additional flags or conditions.

Matrix Transposition

    The print_slot_machine() function transposes the slot machine's column-based matrix into rows for user-friendly visualization.

Input Validation and User Feedback

    Comprehensive input validation ensures a seamless experience. Error messages guide users to provide valid inputs.
    The program gracefully handles edge cases, such as insufficient balance or invalid inputs, maintaining robustness.

Usage Instructions

    Run the Program
    Execute the script in a Python interpreter.

    Deposit Money
    Enter the amount you'd like to deposit. The program ensures the value is valid and greater than zero.

    Place Bets
        Choose how many lines to bet on (1 to 3).
        Enter the amount you'd like to bet per line. Bets must be within the specified range and cannot exceed your total balance.

    Spin the Slot Machine
        View the slot machine's results in a grid format.
        Check your winnings and the lines you've won on.

    Repeat or Quit
        Continue playing with your updated balance or quit at any time to cash out your winnings.

Closing Thoughts

This project represents a step forward in leveraging Python's capabilities to build engaging and interactive programs. By incorporating advanced logic like matrix transposition, probability-based symbol generation, and loop-based validation, the code demonstrates a solid understanding of Python's features and best practices.

Enjoy spinning the reels! 🎰
