## Program Details

- Implement an AI for Minesweeper using a Sentence class for logical statements and a MinesweeperAI class for gameplay.
- It makes safe moves based on known information and random moves if unsure.
- The AI learns from safe moves, updating knowledge and inferring new ones.
- The AI for Minesweeper is built using a logical representation called the Sentence class and a MinesweeperAI class for gameplay.

1. Sentence Class: Represents logical statements about the game state, with methods for handling known mines, known safes, and marking mines or safes.
2. MinesweeperAI Class:
   - add_knowledge: Updates knowledge based on a safe cell's count, marks the cell as safe, updates sentences, and infers new knowledge.
   - make_safe_move: Returns a safe move if known; otherwise, returns None.
   - make_random_move: Returns a random valid move if no safe move is known, ensuring no repeated or risky moves.
3. Process:
   - The AI learns from each safe move, updating its knowledge base.
   - It continuously infers new safe moves or mines based on updated knowledge.
   - If a safe move is guaranteed, it's made; otherwise, it chooses a random move.
