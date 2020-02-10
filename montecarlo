import matplotlib.pyplot as plt
import random    

## increase the default plotsize
from pylab import rcParams
rcParams['figure.figsize'] = 12,6
## dice roll
def diceroll():
    dice = random.randint(1, 100)
    if dice < 52:
        return(False)
    else:
        return(True)
        
        def playy(total_funds, wager_amount, total_plays):
    playnum = []
    funds = []
    ## play number 1    
    play = 1
    while play <= total_plays:
        ## if player wins
        if diceroll():
            ## adding the money to our funds
            total_funds = total_funds + wager_amount
            funds.append(total_funds)
            ## append the play number
            playnum.append(play) 
            
        
        ## if the house wins
        else:
            playnum.append(play)
            total_funds = total_funds - wager_amount
            funds.append(total_funds)
        play += 1       
    
    ## line plot of funds over time    
    plt.plot(playnum, funds)
    finalfund.append(funds[-1])
    return(finalfund)
    
    
finalfund = []
x = 1

plt.figure(figsize = (12,8))
while x <= 100:
    playy(10000, 100, 1000)
    x += 1
    
#Plot the line plot of "Account Value" vs "The number of plays"
plt.xlabel("The number of plays")
plt.ylabel("Account Value")
plt.show()

print("the player starts the game with 10k$ and ends with $", sum(finalfund)/len(finalfund))
