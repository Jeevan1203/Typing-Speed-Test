# Typing Speed Test

This Python code provides a simple typing speed test application. It presents the user with a predefined sentence and measures their typing speed, accuracy, and the time taken.

## Features

* **Test Phrase:** Uses a predefined sentence for users to type.
* **Time Measurement:** Calculates the time taken by the user to type the sentence.
* **Accuracy Calculation:** Determines the accuracy of the user's typing by comparing their input with the original sentence.
* **Speed Calculation:** Computes the typing speed in words per minute (WPM).
* **Results Display:** Shows the total words typed, time used, accuracy percentage, and typing speed in WPM.
* **Retry Option:** Allows users to retry the test multiple times.

## How to Run the Code

1.  Save the code as a Python file (e.g., `typing_test.py`).
2.  Run the file from your terminal using the command: `python typing_test.py`
3.  The test will start, and you'll be prompted to type the given sentence.
4.  After typing the sentence and pressing Enter, the results will be displayed.
5.  You'll be asked if you want to retry.

## Code Explanation

The code uses the following logic:

* **Time Tracking:** The `time` module is used to record the start and end times of the typing test.
* **Input Handling:** The `input()` function takes the user's typed sentence as input.
* **Word Count:** The number of words in both the original sentence and the user's input is calculated using the `split()` method and `len()`.
* **Accuracy Calculation:**
    * It splits both the original string and the input string into sets of words.
    * Then, it calculates the intersection of these two sets. This gives the number of correctly typed words.
    * Accuracy is calculated by dividing the number of correctly typed words by the total number of words in the original string.
* **Speed Calculation:** The typing speed (WPM) is calculated by dividing the number of words typed by the time taken (in minutes).
* **Retry Logic:** A `while` loop allows the user to repeat the test until they choose to exit.
