# AoC 2021: Day 4

Excel still works for Day 4

## Explanations: 
This is a "working" solution without any manual search.
All you need is to correctly import the data and then read the solution.

Works for 100 Bingo cards and up to 100 numbers (0 to 99).

## How it works
Data import is made simple, but as first line is CSV and cards are delimited, import is global for all and some misalignment was possible.
The basic idea is that if you sum the value on a line(or a column, see later), and substract the values that are selected as they appear, reaching 0 means that all number of this line/column has been drawn.
Transposition has been used to keep the same logic as above for column and not for cells.
Then, all one need to check is that for any card, when a new number is drawn that either a line or a colunm reaches 0.
At that moment, we can calculate easily the sum of the remainding number and multiply this by the number that caused this change to 0.
More tricky has been to craft the formulaes to detect the moment this was happening for each card and later between the cards. These are mostly in columns DD to DG.

## Instructions: 
1. Paste raw data, as copied from your puzzle input, in “DATA IN” the sheet at CELL A1
2. Data / “Text to column” with “delimiters” set to “Space” and “Comma” and “Treat consecutive delimiters as one”.
3. Goto to the “SOLUTION” page and read the solutions at cell C1 for part 1 and C2 for part 2

## Additional note:
With this way of working, it is quite easy to figure when a card is fully populated as the calculated above number will reach 0 as there is no remainders ;-) 
