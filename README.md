# ChessWin


You are working directly inside my existing ChessAI GitHub repository.
Before making changes:
- Inspect the existing repository and project files.
- Check my Python installation and environment.
- Check whether Git is configured correctly.
- Identify anything already installed or configured.
- Do not overwrite or delete existing files without checking them first.
Build the project in manageable stages. Prioritise getting a working desktop application before adding advanced features.
Keep terminal commands and responses concise to minimise token usage.
Do not commit or push changes to GitHub without my permission.
Start by checking the environment and reporting any issues before implementing the project.

Build a fully functional, standalone Python desktop application that acts as an advanced chess analysis assistant.

The application must have its own GUI, run locally on Windows and use Python as its primary programming language.
- Python must be the primary programming language.
- This must be a desktop application, NOT a website.
- Opening the application must launch a proper graphical user interface (GUI).
- Use a modular, maintainable architecture.
- Use Stockfish as the chess analysis engine.
- The application must work independently of Chess.com.
- Support Chess.com board recognition in permitted analysis and practice contexts.
- Never require a paid API to perform core chess analysis.
- Do not create unnecessary features, dependencies or complicated architecture.
- Prioritise functionality, accuracy and performance over appearance.
- Do not leave placeholder functions or pretend features work when they do not.
Create a modern, professional interface using PySide6.

Include:
- Chessboard display.
- Start/stop analysis controls.
- Current position display.
- Best move recommendation.
- Alternative moves.
- Evaluation score (+/-).
- Principal variation (suggested move sequence).
- Engine depth and calculation information.
- Settings panel.
- Clear status indicators.
The application must be capable of:
- Detecting a chessboard displayed in a browser.
- Supporting Chess.com.
- Identifying all 64 squares.
- Recognising the pieces and their positions.
- Determining whose turn it is.
- Converting recognised positions into FEN notation.
- Detecting when the board changes.
- Updating the analysis automatically.
Use computer vision where appropriate.

Provide manual board selection and screenshot import as fallbacks.
Integrate Stockfish using python-chess.

The engine must:
- Analyse the current position.
- Identify the strongest available move.
- Provide alternative candidate moves.
- Display evaluation scores.
- Calculate multiple moves ahead.
- Explain recommended moves in understandable language.
- Allow adjustable engine strength and analysis depth.
Display:
- Recommended move visually on the board.
- Highlighted starting and destination squares.
- Best move notation (e.g. Nf3, Qxd5).
- Expected continuation.
- Evaluation before and after the move.
- Explanation of why the move is strong.
Include:
- Start analysis.
- Pause analysis.
- Stop analysis.
- Reset board.
- Import screenshot.
- Load FEN.
- Copy FEN.
- Change engine settings.
Support Chess.com board recognition in its permitted analysis, practice and post-game environments.

Do not automate moves or provide engine assistance during active rated or competitive games.
Use:
- Python 3.12+
- PySide6 — desktop GUI.
- python-chess — chess logic and Stockfish integration.
- Stockfish — chess engine.
- OpenCV — image processing and board detection.
- NumPy — image processing support.
- Pillow — screenshot handling.
Only introduce additional dependencies when genuinely necessary.
The application should look like a premium chess analysis product.

Design inspiration:
- Modern dark interface.
- Minimalist layout.
- Professional typography.
- Smooth interactions.
- Clearly separated panels.
- Green highlights for recommended moves.
- Clean chessboard with recognisable pieces.
Suggested layout:

LEFT: Chessboard.

RIGHT:
- Best move.
- Evaluation.
- Alternative moves.
- Move explanations.
- Engine information.
BOTTOM:
- Analysis controls.
- Engine depth.
- Current status.
- Keep the GUI responsive during engine calculations.
- Run Stockfish in a background worker.
- Avoid unnecessary repeated screenshot processing.
- Only reanalyse when the position changes or settings are adjusted.
- Manage memory and CPU usage sensibly.
- Handle errors without crashing.
IMPORTANT: Keep Claude Code usage and terminal commands efficient.
- Use short, purposeful terminal commands.
- Combine related shell operations where practical.
- Avoid repeatedly inspecting files that have already been inspected.
- Do not dump entire directories or large files into context.
- Read only relevant sections of files.
- Avoid unnecessary explanations between implementation steps.
- Do not repeatedly rewrite working code.
- Reuse existing dependencies and components.
- Do not install packages without checking whether they are already installed.
- Avoid unnecessary planning documents.
- Keep responses concise and focus on implementation.
- Work autonomously unless an important decision genuinely requires my input.
Create a clean project structure similar to:

chess_assistant/
main.py
requirements.txt
README.md
config/
gui/
engine/
vision/
chess/
assets/
utils/

Keep each component separate and organised.
Work through these stages:
1. Inspect the environment and check Python installation.
2. Create the project structure.
3. Install and configure dependencies.
4. Integrate Stockfish.
5. Build the desktop GUI.
6. Implement chessboard functionality.
7. Implement screenshot-based board recognition.
8. Implement FEN extraction.
9. Connect board recognition to the chess engine.
10. Add move visualisation and explanations.
11. Test all functionality.
12. Fix errors and optimise performance.
Do not stop after creating a basic prototype.
Before declaring the project complete:
- Confirm the application launches.
- Confirm Stockfish works.
- Test multiple chess positions.
- Verify FEN generation.
- Test board recognition with different board themes.
- Test both white and black orientations.
- Verify recommended moves against the engine.
- Test GUI responsiveness.
- Test error handling.
I want a working Windows desktop application.

Provide:
- Complete Python source code.
- requirements.txt.
- Stockfish setup instructions.
- A simple installation process.
- A README.
- A way to launch the application using a desktop shortcut or executable.
Start by inspecting the environment, then build the application. Prioritise a working end-to-end product over unnecessary complexity.
