
# Chess Adventure ♟️

A Python-based chess game designed to run smoothly in Kaggle notebooks without requiring ipywidgets. The project provides a visual chessboard, move validation, move history tracking, and an easy-to-use interface for playing chess directly within a notebook environment.

## Features

* Interactive chess board visualization
* Standard chess piece representation using Unicode symbols
* Legal move validation
* Move history tracking
* Pawn promotion
* Turn-based gameplay
* Board coordinate labels (a–h, 1–8)
* Kaggle-compatible implementation
* No ipywidgets required



## Technologies Used

* Python 3
* IPython Display
* HTML/CSS rendering inside notebooks

## How to Start

Create a game instance:

```python
game = ChessGame()
```

Display the board:

```python
game.show_board()
```

View possible moves for a piece:

```python
game.show_moves("g1")
```

Make a move:

```python
game.move("e2", "e4")
```

Reset the game:

```python
game.reset()
```

## Example Gameplay

```python
game.move("e2", "e4")
game.move("e7", "e5")
game.move("g1", "f3")
```

## Future Improvements

* Check detection
* Checkmate detection
* Stalemate detection
* Castling
* En passant
* AI opponent
* Move timer
* Multiplayer support






