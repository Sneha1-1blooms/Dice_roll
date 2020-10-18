# Dice_roll
import random
def main():
    player1=0
    player1wins=0
    player2=0
    player2wins=0
    round=1
    while round !=4:
        print('Round ' + str(round))
        player1=dice_roll()
        player2=dice_roll()
        print('player1 roll : ' + str(player1))
        print('player2 roll :  ' + str(player2))
        if player1==player2:
            print('Draw!')
        elif player1>player2:
            player1wins=player1wins+1
            print('player 1 wins!')
        else:
            player2wins=player2wins+1
            print('player 2 wins!')
        round=round+1
    if player1wins==player2wins:
        print('Draw!')
    elif player1wins>player2wins:
        print('player 1 wins - Round won : ' + str(player1wins))
    else:
        print('player 2 wins - Round won : ' + str(player2wins))
        
        
    
        
def dice_roll ():
    dice_roll=random.randint(1, 6)
    return dice_roll
main()
    
