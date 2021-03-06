# BlackJack
Console-based BlackJack Card Game in Python. Oodles of Fun.

If you already have python3 installed, run the file in your console with the command
```
python3 BlackJack.py
```
to experience this classic card game!

To check what version of python is installed, type ```python --version ``` into your terminal.

I stored the cards and card values in a dictionary called Cards. I stored the suits in a list called suits. In the beginning, I generate a generic deck of cards of thirteen values and four suits. I shuffle a list called mask in my function deal_cards to create a unique deck each time the code is run. To shuffle this list, I instantiate an object from python's random library because it's easy and convenient to. use. 

The edge case that was most problematic to account for was the fact that aces have the value of 1 and 11. I added several if-families to deal with this case.

The functions dealer_action and player_action drive the gameplay. dealer_action determines the dealer's score, and player_action allows the player to hit - build up their point total - to reach 21. 

In terms of gameplay, I  followed the BlackJack rules from the website https://wizardofodds.com/games/blackjack/basics/. In the beginning, the dealer and the player are each dealt two cards. The dealer reveals  one of these cards to the player. The player can then decide if they choose to hit or stand. If they choose to hit, they are dealt a new card. If the sum of this card with their previous point total is greater than 21, they go bust and lose. If this is not the case, then the player can hit as many times as they want or until they go bust. When the player chooses to stand, it is the dealer's turn to act. The dealer will always hit if their point total is 16 or less. If the dealer goes bust (their point total is greater than 21), the player wins. If neither the player nor the dealer goes bust, then whoever is closest to 21 wins. If the player and the dealer tie, it goes to a new game. 

I hope you enjoy playing!

