# sudoku-solver
Solves a Sudoku puzzle and prints its solution

## Introduction
A Sudoku puzzle is played on a 9 x 9 grid where some cells are already filled.
The object of the game is to fill every blank cell with numbers 1,2,3,...,9 so that:
- no row has repeated values
- no column has repeated values
- no 3 x 3 block has repeated values

Given a Sudoku puzzle, this program prints a solution if it exists.

## Install
Requires:
- Common Lisp installation
- Roswell build system
- `alexandria` and `cl-str` packages from Quicklisp

(Optional) This program can be compiled by executing `ros build sudoku.ros`.

## Use
On the command line, execute `./sudoku.ros input-file` with your input file.

A sample Sudoku puzzle is provided in `sudoku.txt` (from Wikipedia).

**Input format**

A text file with
- each row on a separate line with filled in numbers
- blank entry for empty cells

```
5,3,,,7,,,,
6,,,1,9,5,,,
,9,8,,,,,6,
8,,,,6,,,,3
4,,,8,,3,,,1
7,,,,2,,,,6
,6,,,,,2,8,
,,,4,1,9,,,5
,,,,8,,,7,9`
```
**Example output**
```
 5 3 4 6 7 8 9 1 2
 6 7 2 1 9 5 3 4 8
 1 9 8 3 4 2 5 6 7
 8 5 9 7 6 1 4 2 3
 4 2 6 8 5 3 7 9 1
 7 1 3 9 2 4 8 5 6
 9 6 1 5 3 7 2 8 4
 2 8 7 4 1 9 6 3 5
 3 4 5 2 8 6 1 7 9
 ```

## Author, License
Copyright (C) 2020 Alan Tseng

GNU General Public License v3
