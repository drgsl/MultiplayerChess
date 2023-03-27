# 🎲 Multiplayer Console Chess built with Sockets in C

This project is a two-player console-based chess game built using sockets in C. 
The game allows players to connect to a server and play a game of chess with each other.

<img align="right" src="https://github.com/BobuDragos/MultiplayerChess/blob/main/TCP%20Explained.png" width="20%" />

## 🎥 Showcase
Check out this [YouTube video](https://www.youtube.com/watch?v=Vd_fVtrs2P8&list=PL-j3UE1st04DPCC_Em-48laJLwJhntyAW&index=1&t=2s&ab_channel=dragosel505) to see the project in action!

## 🕹️ How to Play
To play the game, you need to first build and run the server and then connect two clients to it.

## 💻 Linux Build
To compile this project, run the `./build.sh` command to generate the executable files.

To launch the server, use the `./server` command.

For each client you want to connect, execute the `./client 127.0.0 5005` command.

## 🛠️ Overview
This project consists of three components:


<img align="left" src="https://github.com/BobuDragos/MultiplayerChess/blob/main/chessServerDiagram.png" width="40%" />

### Server Script
The Server Script acts as a supervisor for the game of chess. It creates a socket for the two clients to connect to and then forks and creates a session for them. The server serves as a central point for both clients, as it relays the moves between them. 

### Client Script
The Client Script requires an IP and port to connect to the server, and each client receives the other's move from the server before sending their own move. 

### ChessBoard Script
The Chessboard contains all the functions related to the game of chess, from printing the board to validating moves for each piece. It also checks if either king has been captured, although there are no checks in this game mode.

## 🚀 Future Development
- Adding game mode with check detection
- Adding an AI mode
- Adding an option for players to save and load games

## 🎖️ Credits
This game was developed for the Computer Networks course in the Computer Science Bachelor's program, 
with guidance from our professor and support from the Alexandru Ioan Cuza Iasi faculty. 

## 🤝 Contact
If you have any questions about this repository or would like to get in touch with Dragos A. Bobu, 
feel free to reach out to his [email](mailto:bobudragos0@gmail.com?subject=[GitHub]TCPChess%20Interest) or [website](https://bobudragos.github.io/).

Feel free to contribute to this project and improve it further.
