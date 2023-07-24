https://echohatch1.medium.com/making-a-simple-blackjack-game-with-html-and-javascript-5124123762ce



card = suit & rank is a

const card is an object made of a suit, rank, with a set value (except for Ace), has no duplicates, is randomly ordered throughout the deck




Descriptor
Resources
Future Developments
Current Bugs under Development


A. PHASES
   1. "Pure" text/code based
   2. 


B. 

 1. Pseudocode components and methods
        a) Loops
        b)
    2. Classes to create and code for
    3. Buttons, Cards, and Visual Elements 







Getting Started
Live Server Extension
Create Cards - HTML
Create the Game Play Grid
Create Cards Dynamically - JS Code
Initialise Card Positions
Load Game and Start Game
Stack Cards
Flip Cards
Shuffle Cards
Deal Cards
Choose Card
Styling and Layout
Animation
Responsive Layout
Local Storage
<ul










Steps
Wireframing("preFlopped")
Components


Phases

Pure Text based


does it function
multipple rouunds 
multiplayer

win and lose state



essential steps
1. place first card to player
2. place second card to player
3. add two cards, provide sum


## Blackjack

Game build

## RESOURCES ##
1. (StepbyStep) https://scrimba.com/playlist/p3py7U7


2. (VIDEO) Code Blackjack with JavaScript HTML CSS
Kenny Yip Coding
https://www.youtube.com/watch?v=bMYCWccL-3U


3. https://www.thatsoftwaredude.com/content/6417/how-to-code-blackjack-using-javascript

4. https://math.hws.edu/eck/cs271/js-work/Blackjack.html


5. https://code-boxx.com/javascript-blackjack/


Create a deck
shuffle it
deal cards to the dealer and the player
keep running sum of each hand
optimize/adjust value of ace from 1 to 11
if you have blackjack —ace of spades and jack of spades, automatically win
dealer forced hit option if under 16 (adjustable to 15 and 17)
if you get five cards without going over, you win


option to hit (draw additional cards) or stay (hold at current sum and submit hand for compare count)

bid option to adjust value of hand bet for current hand

counting cards option (running counting cards option to maximize bet)


steps

1. create deck of cards
2. optional shuffle deck
3. buttons for number of players on start screen (additional players have various AI personalities)
4. shuffle button
5. 



CONDITIONALS INDEX (Precedence here is critical)
1. Lose Conditions (over 21)
        a. Under 21, but player's hand is less than dealer's hand, which is less than or equal to 21 at count check (countCheck)
2. Lose Conditio



Developer Notes:

Namimg of assets can play a critical role in the architecture of coding design (note: structure of naming convention for cards is conducive towards randomized shuffle and selection syntax)


Issues, challenges, missteps:

One of the biggest challenges as a developer can often come from a simple or easily corrected oversight or mistake, that ideally ample repetition will reduce the risk of repeating. One such example is forgetting to include the script src reference link in the html head. 


What is span tag? used in creating dealer and user sum

sizing or non-responsive html issues to styling are likely an issue with improper tag syntax, placement, or closing (or lack thereof)


????
span
“#” in css style sheet as specific styling “tag"

 let temp = deck[i];
        deck[i] = deck[j];
        deck[j] = temp;


PROJECT
Non-negotiables:
Win State
Lose State
Competitor (computer or alternate player)
Randomization process
Reset game function
Restart function
Memory system (for Deck and Cards Played)
Flexbox incorporation
ReadMe with credits



Stretch Goals:
Additional Players
Visual Shuffling Effect
AI programmable personality to additional “players"
Memory System (for Bets submitted)
Player “Fold” option, based on bet placed (to counteract/limit wins)
Pure Javascript based Game
Symbols for each suit in text?
**optimize for strategy, memory, bluffing, and cunning **
Alternative randomization approaches for deck? 
High Score record in memory?
Flexbox visual effects



** Moments of Elegance/Coding Brilliance ie Eloquent Javascript:

Assets naming convention for conversion into randomization naming  scheme

Background:
-minimal actual coding experience, mostly app based tutorials and lessons for past year

Rational for Game selection:
Wanted a project that I could build on, share, experiment with, and create a practical use for; in this case, learning how to count cards and discovering more effective strategies for playing black jack

alternative options: poker, and flash cards for memory improvement


LESSONS:

For Better Coding as a Developer:
Always add comments and notes adjacent to loops to demonstrate what their expected output will appear like


ERRORS, CHALLENGES, FRUSTRATIONS:

Had copied verbatim randomization technique from tutorial and coulnt for the life of me get it to work

What are the arrows of the flowchart of your code (ie shuffleDeck on windowonload, connected and sourced to functions for creating random sort of cards)

Why is the SKELETON created a certain way?


<!-- 
    while (dealerSum < 17) {               // create while loop to repeatedly evaluate if the dealer should "hit" for a new card
            // <img>                        // 
            let cardImg = document.createElement("img");
            let card = deck.pop();
            cardImg.src = "./cards/" + card + ".png";
            dealerSum += getValue(card);
            dealerAceCount += checkAce(card);
            document.getElementById("dealer-cards").append(cardImg); -->




REVERSE ENGINEERING LOGIC:


    <!-- while (dealerSum < 17) {               // create while loop to repeatedly evaluate if the dealer should "hit" for a new card
            // <img>                        // 
            let cardImg = document.createElement("img");
            let card = deck.pop();
            cardImg.src = "./cards/" + card + ".png";
            dealerSum += getValue(card);
            dealerAceCount += checkAce(card);
            document.getElementById("dealer-cards").append(cardImg); -->