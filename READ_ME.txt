card_rand v1.0
Created by MonsieurWaffle
Hope you enjoy!

--CHANGELOG--
v1.0 - Basic functionality.
v1.0.1 - Ensured varibles conformed to naming conventions, added docstirngs.

--ABOUT--
Thanks for using card_rand!
This module allows you to:
- Eaisily draw and count playing cards 
- Check for repeat cards
- Count the values of drawn cards
- Give the user a choice as to the value of an ace

--USE--
- Ensure the card_rand module is in the same directory as your script.
- Import the module by typing 'import card_rand'.
- Create a list in your script with the name 'played_cards'.
- To use a method, write 'card_rand.' before the name of the method, e.g. card_rand.test().
- To use the returned values from a method, use this layout -> return_value1, return_value2 = card_rand.method_name()
- Before use, test the module is correctly functioning by calling the 'test' method.


--METHODS--

test():
    Function - Checks if the module is functioning correctly by prining a short phrase.

    Parameters:
        None
    
    Return values:
        None


cardChecker():
    Function - Checks if a card has been drawn. If not, it is added to the list of drawn cards.

    Parameters:
        drawn_card - The card you wish to check.
        played_cards - The cards that have already been drawn.

    Return values:
        played_cards - The updated list of drawn cards.
        is_viable - Will return True if the card has not yet been drawn.
    

drawCard():
    Function - Draws a playing card, provides a str representing the drawn card, as well as a current score. Will never draw the same card twice.
    
    Parameters:
	current_score - The current total of the drawn cards.
	played_cards - The list of drawn cards.
	ace-choise - Weather or not the user can choose the ace value. (Takes either True or False.)

    Return values:
	current_score - The updated total of the drawn cards.
	display_card - A string representing the drawn card.
	played_cards - The updated list of drawn cards.