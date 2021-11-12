# AlphaGo-Demo
COMP7404 Group Project Demo

This is a replication of AlphaGo based on brilee's project MuGo(https://github.com/brilee/MuGo)
I made a small change in go.py trying to solve a theoretical problem the author mentioned in strategy.py which is the AI in MCTS mode will eventually fill its own eyes.
I added a move_to_fill_eye function in go.py to check if the AI is filling its own eyes at endgame, which is always meaningless and even harmful.
To be noticed, this is not the best way to solve this problem because technically speaking filling one's own eye is stupid but not illegal. Thus it would be better to fix it from the strategy level, not the go level.
