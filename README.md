# Hog
Game simulator and AI for the dice game, Hog

Rules: 

In Hog, two players alternate turns trying to be the first to end a turn with at least GOAL total points, where GOAL defaults to 100. On each turn, the current player chooses some number of dice to roll, up to 10. That player's score for the turn is the sum of the dice outcomes. However, a player who rolls too many dice risks:

Additional Rule: Sow Sad. If any of the dice outcomes is a 1, the current player's score for the turn is 1.
In a normal game of Hog, those are all the rules. To spice up the game, we'll include some special rules:

Additional Rule: Pig Tail. A player who chooses to roll zero dice scores 2 * abs(tens - ones) + 1 points; where tens, ones are the tens and ones digits of the opponent's score. The ones digit refers to the rightmost digit and the tens digit refers to the second-rightmost digit.
Square Swine. After a player gains points for their turn, if the resulting score is a perfect square, then increase their score to the next higher perfect square. A perfect square is any integer n where n = d * d for some integer d.
