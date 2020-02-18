# CeeChess
Hi! I am a bot written in C, heavily inspired by the Vice engine and video series done by Bluefever! If you want to try your hand at facing me, I am on lichess at https://lichess.org/@/seeChessBot!

**Rating:**

Version 1.2 Rating:
```
Rank      Name         Elo    +   -   games   score    oppo.  draws
 1    SeeChess_v1.2  : 2212   21  21   802    60.5 %   2139   28.9 %
 2    MORA_1.1.0     : 2207   35  35   268    49.1 %   2213   31.0 %
 3    Raven0.50      : 2139   37  37   267    39.5 %   2213   24.3 %
 4    Vice10-64      : 2066   36  36   267    30.0 %   2213   31.5 %
```
Version 1.3 Rating:
```
Rank      Name         Elo    +   -   games
 1    CeeChess-v1.3  : 2310   19  19  1000
 2    SeeChessTapered: 2238   17  17  1000
 3    SeeChess-v1.2  : 2212   17  17  1000  
```

# Engine Features

**Search:**
The Engine searches with a Principal Variation Search inside a Negamax framework

**Lossless Pruning:**
- Alpha-Beta pruning
- Mate Distance pruning

**Lossy Pruning:**
- Transposition Table
- Razoring
- Null Move Pruning
- Late Move Reductions
- Futility Pruning
- Static Null Move Pruning (Reverse Futility Pruning)

**Move Ordering:**
- PV Move
- Transposition Table Ordering
- Captures ordered by MVV/LVA (Most Valuable Victim/Least Valuable Attacker)
- 2 Killer Moves
- History Ordering

**Evaluation:**
- Material
- PSQT (Midgame and Endgame, from Lyudmil)
- Bishop pair heuristic (for Midgame and Endgame)
- Passed Pawn evaluation (Midgame and Endgame tables)
- Isolated pawn heuristic
- Open file heuristics (for Rook and Queen)
- Tapered evaluation

**Planned Improvements (ordered by perceived feasibility):**
- Polyglot Opening Book
- Syzygy Tablebases
- Mobility

**Other Possible Improvements (No particular order):**
- IID (Internal Iterative Deepening)
- Futility Pruning
- SEE (Static Exchange Evaluation)
- Bitboards
- King Safety
- Aspiration Windows

None of the code I write is copyrighted or protected in any way, and you may make use of all that you wish. You do not have to credit me if you use any of the code I write, but it would be great if you did
