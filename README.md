# Text-Parser


A small command-line Python project that explores a text sample and reports a few useful details. It is designed as a beginner-friendly exercise in strings, lists, dictionaries, and console input.

## What it does

When you run the program, it asks for a text sample and three search strings. It then:

- Counts each search string in the sample (matching is case-insensitive).
- Counts words by splitting the sample on whitespace.
- Shows the first and last character of the sample.
- Reverses the order of the words and prints the result.
- Checks whether the text `python` appears in the sample (case-insensitive).

## Requirements

- Python 3
- No third-party packages

## Run it

Open a terminal in the project directory and run:

```bash
python main.py
```

On some systems, use `python3 main.py` instead.

### Example

```text
Enter a text of your choice: Python makes text processing fun
Enter the first letter: t
Enter the second letter: p
Enter the third letter: z

LETTER REPETITIONS
We have found the letter 't' repeated 1 times
We have found the letter 'p' repeated 2 times
We have found the letter 'z' repeated 0 times

NUMBER OF WORDS
We have found 5 words in your text

FIRST AND LAST LETTERS
The initial letter is 'p', the final letter is 'n'

INVERTED TEXT
If we order your text backwards it will say 'fun processing text makes python'

LOOKING FOR THE WORD PYTHON
The word 'Python' was found in the text
```

## Project structure

```text
Text-Parser/
├── main.py       # Interactive text analysis program
├── README.md     # Project overview and usage instructions
└── .gitignore    # Files that should not be committed
```

## Notes and current limitations

- The three search inputs are counted as entered; they are not restricted to one character, so a multi-character input is counted as a substring.
- The `python` check looks for that sequence anywhere in the text, including inside a longer word.
- Entering an empty text currently causes an error when the program tries to display its first and last characters.

## Possible next steps

- Handle empty input gracefully.
- Validate that each search input contains exactly one character.
- Report whether `python` appears as a separate word.
- Add automated tests or a reusable function interface.

## License

No license has been selected yet. Add a license before publishing if you want to define how others may use, modify, or redistribute the project.
