# Chess-AI
Won second position in Sanskriti School Project Beta 6.0 in 2022. 

https://drive.google.com/drive/u/0/folders/1k6kgBQ_FIKxEN6LZProvFIDP0jJGMupI

School Name: - K.R. Mangalam World School, Vikaspuri
Team Members: - Pratham Chugh, Jashanveer Singh Arora, Kyna Rathaur, Parth Dua, Ansh Goel

Input Format : You have to enter the coordinates of chess. Given is the example of chess board. 
Eg : 
Enter your move :
From where do you want to move the piece ? (Eg : a2 ) Enter the cordinates of chess. : b2
To where do you want to move that piece ? (Eg : a3 ) Enter the cordinates of chess.  : b4


We have created a Chess AI bot using Min-Max algorithm and python-chess module. We have used Minmax algorithm in unique way with only loops and python’s basic data structures. 

We have analysed the value of the board by designating each piece a specific value.
To make the best possible move, our AI bot would calculate all the possible outcomes of the next 3 moves being its move then opponents move and then again AI’s move. It will add value of each piece in AI’s turn and subtract value of each piece in opponent’s turn to the score variable. It will then form nested lists (which represent a tree like data structure) and start with minmax algorithm. 

Min-Max Algorithm
The AI bot will find the maximum score of all the possible moves in its own turns and minimum value of all the possible moves for the opponent’s turns.  It will then see the best move to be played according to the most optimal values from the Min-Max Algorithm.
It calculates the value of the board for every 3rd move ahead and then the maximum value of the 3rd layer gets assigned to the 2nd move layer. Then it calculates the minimum of all the 2nd layer moves and assigns it to the 1st layer. To calculate the optimal, move the maximum value is taken form the 1st layer.
If there are multiple values with the same most optimal score, then it selects random move from the list of all the most optimal scores. 
Checkmate
At every move, the bot will check if it is a possible condition for checkmate, and if it is opponent’s checkmate, it will append a very high value to the nested lists (representing tree like data structure) because there is a very high chance that it will be the most optimal move. If the opponent is giving our bot the checkmate at that particular location, it will append a very low value to the nested lists (representing tree like data structure) because it would want to surely avoid that losing situation. 


