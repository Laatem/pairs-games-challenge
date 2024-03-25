# pairs-games-challenge

## Principle

For each turn, the user must provide coordonates (example A1 or C7) to reveal a map, then another to find the right pairs, if the cards are identical they will stay visible, otherwise they will turn back and game continue

## Step
- Create a gid with column and row for the coordonates
- Create a data structure for the game
- Manage all keyboard entries for the game process
- Develop the logic of the game
- Create a .yml configuration file
- Implement a function to save and load a game

**Bonus** : Create a difficulty mode (easy / hard) to handle a higher number of moves per level

## Conditions
- The display must done using command line
- Handle the clearing of the command line after each use
- Handle exceptions of users entries
- Identify the grid with numbers for rows and letters for columns (from 1 to 10 and from A to J)
- The database must be handle using tinydb
- Use the Memento design pattern to handle load / save
- A new game start to level 0 (2x2 grid) to level 4
```
level 0 : 2 x 2
level 1 : 4 x 4
level 2 : 6 x 6
level 3 : 8 x 8
level 4 : 10 x 10
```

## Configuration file

- grid_level: size of the grid by level
- front : symbol for the visible side of card
- back : symbol for the back of card
```
level: [2, 4, 6, 8, 10]

recto: [" 😯", " 😀", " 😁", " 🤣", " 😉",
        " 😎", " 😍", " 🤗", " 🤩", " 😑",
        " 🙄", " 😣", " 😏", " 😮", " 🤐",
        " 😫", " 😴", " 😛", " 🤤", " 😓",
        " 🙃", " 🤑", " 🥵", " 🥶", " 😤",
        " 😭", " 🥳", " 😨", " 🤯", " 😱",
        " 🤪", " 😵", " 😡", " 🥺", " 😷",
        " 🤕", " 🤢", " 🤮", " 😇", " 🤠",
        " 🤥", " 🧐", " 😈", " 🤡", " 👻",
        " 🤘", " 🐍", " 🦆", " 🦁", " 🎮"]

verso: " ❓"
```