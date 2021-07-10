#Tuples are not changable, we can use list or dict

board = [" " for i in range(9)]
#print(board)


def game_board():
    row1 = "|{}|{}|{}|".format(board[0],board[1],board[2])
    row2 = "|{}|{}|{}|".format(board[3],board[4],board[5])
    row3 = "|{}|{}|{}|".format(board[6],board[7],board[8])

    print(row1)
    print(row2)
    print(row3)
    
def player_move(icon):
    if icon == "X":
        number = 1
    elif icon == "O":
        number = 2

    print("Your turn player{}".format(number))
    choice = int(input("Enter your move: ").strip())
    print(choice)
    if board[choice -1] == " ":
        board[choice -1] = icon
        
    else:
        print()
        print("This is already occupied")

def winner(icon):
    if(board[0] == icon and board[1]== icon and board[2]== icon)or\
                (board[3]== icon and board[4]== icon and board[5]== icon)or\
                (board[6]== icon and board[7]== icon and board[8]== icon)or\
                (board[0]== icon and board[3]== icon and board[6]== icon)or\
                (board[1]== icon and board[4]== icon and board[7]== icon)or\
                (board[2]== icon and board[5]== icon and board[8]== icon)or\
                (board[0]== icon and board[4]== icon and board[8]== icon)or\
                (board[2]== icon and board[4]== icon and board[6]== icon):
        return True
    else:
        return False
        
def draw():
    if " " not in board:
        return True
    else:
        return False
        
        
           
        
while True:
    game_board()
    player_move("X")
    game_board()
    if winner("X"):
         print("X -- CONGRATS  you won the game!!!")
         break
    elif draw():
         print("It's a Draw")
         break
        
    player_move("O")
    if winner("O"):
        print("O -- CONGRATS  you won the game!!!")
        break
    elif draw():
        print("It's a Draw")

    
while False:
    print("Try another game")
    break
