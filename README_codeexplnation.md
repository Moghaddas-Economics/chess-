part 1:  Program Initialization


| Function                  | Purpose                                                                         |
| ------------------------- | ------------------------------------------------------------------------------- |
| `display`                 | Displays the HTML chessboard in the notebook.                                   |
| `HTML`                    | Converts the generated HTML code into a formatted chessboard.                   |
| `clear_output(wait=True)` | Clears the previous board before showing the updated one.                       |
| `SYMBOLS`                 | Maps letters (e.g., `K`, `q`) to Unicode chess symbols (♔, ♛).                  |
| `create_board()`          | Creates the initial 8×8 chessboard with all pieces in their starting positions. |
| `is_white(piece)`         | Returns `True` if the selected piece belongs to White.                          |
| `is_black(piece)`         | Returns `True` if the selected piece belongs to Black.                          |

part 2: helper functions and move prepration

| Function                       | Purpose                                                                   |
| ------------------------------ | ------------------------------------------------------------------------- |
| `is_empty(piece)`              | Checks whether a square contains no chess piece.                          |
| `is_on_board(row, col)`        | Verifies that a position is inside the 8×8 board.                         |
| `is_enemy(piece, white_turn)`  | Determines whether a piece belongs to the opponent.                       |
| `is_friend(piece, white_turn)` | Determines whether a piece belongs to the current player.                 |
| `square_to_position(square)`   | Converts chess notation (e.g., `e2`) into array coordinates.              |
| `position_to_square(row, col)` | Converts array coordinates back into chess notation.                      |
| `get_moves(board, row, col)`   | Starts the process of calculating all legal moves for the selected piece. |

part 3: pawn and knight movement

| Piece                   | Movement Rule                                                                             |
| ----------------------- | ----------------------------------------------------------------------------------------- |
| **Pawn**                | Moves forward one square if empty.                                                        |
| **Pawn (first move)**   | May move forward two squares from its starting position if both squares are empty.        |
| **Pawn Capture**        | Captures one square diagonally to the left or right.                                      |
| **Knight**              | Moves in an L-shape (2 squares in one direction and 1 square perpendicular).              |
| **Knight Special Rule** | Can jump over other pieces and only cannot land on a square occupied by a friendly piece. |
