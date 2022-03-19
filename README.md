# Codewars-6kyu-GamblingGameJoker_python
Gambling Game Joker


Popular gambling game Joker consists of drawing 6 balls from a drum on which are written numbers between 1 and 45. The winning joker number is formed from the drawn numbers so that in the same order in which the balls are drawn, we write down their last digits.

For example, if the numbers 12, 35, 1, 2, 23 and 39 are drawn in order, then it is a joker No. 251239.

1[2], 3[5], [1], [2], 2[3], 3[9] --> 251239

Players buy winning tickets and look forward to drawing and calculating the joker number to calculate their possible gain. The winnings of the ticket are calculated by comparing the serial number written on the ticket with the calculated joker number in a way to count how many last digits of these two numbers match, as shown in the following table.

Serial No. | Name of prize
-----------+---------------
251239     |   I type
X51239     |   II type
XX1239     |   III type
XXX239     |   IV type
XXXX39     |   V type
XXXXX9     |   Losing card
XXXXXX     |   Losing card
In the left column are the serial numbers of the tickets, where X denotes arbitrary digits. In the right column of the table are the winnings names for each of the serial number forms. So if the serial number is exactly equal to the Joker number then we get the gain of type I, if the last 5 digits are equal we get the gain of type II, and so on, until the gain of type V, the kind we get when the last two digits are equal. All other serials are not winning.

Write a program that will return the names of the winnings for a given Joker number and given tickets. The names of the winnings must be written exactly as written in the table above (the number of winnings is written in Roman numbers with capital letters ‘I’ and ‘V’, followed by a space and lowercase letters ‘type’).

Input
joker_nums --> an array of 6 numbers from which you have to make the winning Joker number

ticket_serials --> an array of 3 ticket serial numbers

Output
You should return a list with the names of the winnings for the 3 given tickets

joker_card([12, 35, 1, 2, 23, 39], ['151239', '251229', '251339']) --> ["II type", "Losing card", "V type"]
Note
some tickets may have leading zeros
some joker numbers may have leading zeros
leading zeros still count towards the total

https://www.codewars.com/kata/621e323a98afab001628d9a0/train/python  
   
   
   
