# Tic Tac Toe Gamer Runner Using WebAssembly
This project is a simple Tic Tac Toe game runner implemented using WebAssembly (Wasm). The game allows users to play Tic Tac Toe in their web browser directly through the execution of WebAssembly code written in WebAssembly Text Format (WAT). The compiled binary is run using "go get github.com/wasmerio/wasmer-go/wasmer" runtime as it stores the previos state of the players unlike "wasmtime" runtime.

## Demo:
```
$ wat2wasm tictactoe.wat

$ go run tictactoe-runner.go 
Tic Tac Toe Runner

---------------------

---.---.---.
|   |   |   |
|   |   |   |
|   |   |   |
`---^---^---'

[X's turn] enter row,col -> 1,1
.---.---.---.
|   |   |   |
|   | X |   |
|   |   |   |
`---^---^---'
[O's turn] enter row,col -> 0,1
.---.---.---.
|   | O |   |
|   | X |   |
|   |   |   |
`---^---^---'
[X's turn] enter row,col -> 1,2
.---.---.---.
|   | O |   |
|   | X | X |
|   |   |   |
`---^---^---'
[O's turn] enter row,col ->
```
