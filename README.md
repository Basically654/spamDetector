# **Spam Detector**
## Description
This Java program reads a list of spam keywords from "spamList.txt" and checks a text file "spam.txt" for potential spam phrases. If any keyword is found in the text, it flags the text as potential spam.

## Usage
Ensure you have the Java runtime environment installed.
Place the list of spam keywords in a file named "spamList.txt".
Provide the text to be checked in a file named "spam.txt".
Run the fileReader program.
## Features
Case-insensitive matching: The program converts both the spam list and the text to uppercase for case-insensitive matching.
Customizable spam list: Easily update the list of spam keywords in the "spamList.txt" file.
## How it works
Reads the spam keywords from "spamList.txt" and converts them to uppercase.
Reads the text from "spam.txt" and converts it to uppercase.
Checks for each keyword in the text and counts the occurrences.
If at least one keyword is found, the program flags the text as potential spam.
## Notes
The program assumes a simple keyword matching approach and does not consider variations or context.
