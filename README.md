# AlphaGo-Demo
COMP7404 Group Project Demo

This is a replication of AlphaGo based on brilee's project MuGo (https://github.com/brilee/MuGo)
I changed the file go.py trying to solve the theoretical problem the author mentioned in strategy.py which is the AI in MCTS mode will eventually fill its own eyes.
I added a move_to_fill_eye function in go.py to check if the AI is filling its own eyes at endgame, which is always meaningless and even harmful.
To be noticed, this is not the best way to solve this problem because technically speaking filling one's own eye is stupid but not illegal. Thus it would be better to fix it from the strategy level, not the go level.

Make sure to check brilee's requirements.txt. It would require a lot of excessive work if you do not get the compatible version at first.
My setting: conda 4.10.3  python 3.6.13  tensorflow_gpu 1.15.0  cuda 9.0  cudnn 7.0.5
My project is based on Windows OS & Anaconda, so some of brilee's commands do not work for me, most of which are related to gogui and gnogo. I have upload a file with common commands under Anaconda environment.
