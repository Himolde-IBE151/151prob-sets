# Hangman Game
Problem Sets IBE151 HiM

In this assignment you will implement a Hangman Game.

As in the previous task, you will receive a template, with some declared functions that you will complete.
To access the template,

Install git if you haven't done it before.
open the terminal (git-bash in Windows)
create a folder for your programming tasks (mkdir foldername),
enter that folder (cd foldername), then run:
git clone -b hangman https://github.com/Himolde-IBE151/prob-sets.git hangman
You are given a function (get_words()) that, when called, returns a random word from a list of words. That function is available in module words, you just need to import words and called the get_words() function inside this module as:

import words
random_word = words.get_words()
Our version of the game works like this: you get a word from function get_words() that should be guessed by the user. In the code above that word has been assigned to variable random_word. You will print 3 underscores ('_')  for every letter on the word. For instance, if the word is "Galaxies" you print

___ ___ ___ ___ ___ ___ ___ ___

Then you ask the user to type a character on the keyboard. If the character  is on the word, you will print the word replacing the ___ by the letter typed. For example, if the character typed was an "a" the program should print:

___  a  ___  a  ___ ___ ___ ___

If all the word has been completed print " You won! 😀" and the game ends.

If the letter typed is not in the word, print the word the way it is at that moment, the last letter typed below and how many chances (s)he got left. Ex. if the user typed 'a' 'l' 'x' 'z'  't' it should be printed:

___  a   l  a  x  ___ ___ ___

z t 

" You have 5 attempts left"

and update the hanged man drawing. You can use the functions provided in the template to draw a hangman. 

You can assume 10 attempts is the maximum number of characters the user can try. If the user runs out of chances, the program prints " You lost! 😢" and then the complete word.

This assignment is mandatory.  It can be submitted in groups of max 2 students. Choose your Hangman Group inside Canvas/People (one of the IBE151_2020_Teams_of_two teams).  Start early and don't miss the deadline!


