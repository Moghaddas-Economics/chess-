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
