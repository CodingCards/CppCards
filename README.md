<h1 align="center">
    <img align="center" alt="Coding Cards" width="50%" src="https://codingcards.org/static/img/logo/Coding_Cards_Logo_and_Text.svg" />
</h1>

--------

## What is Coding Cards 

**[Coding Cards](https://codingcards.org)** is a web application for learning C++ features in the style of flashcards.
It is also possible to use the built-in editor/compiler to test your solution and play around.

It started as a hobby project with a static set of cards, but we got so much positive feedback that we decided to add an option for the community to create new cards.  


Website: https://codingcards.org


## How to add Cards to the Project
The project structure:

    .
    ├── C++11
    │   ├── card_name-description.md            #Short description (exercise)
    │   ├── card_name-solution.md               #The solution and a link to the cppreferenz page
    │   ├── order.txt                           #File with the order of the cards... don't modify this file
    │   └── ...
    ├── C++14                   
    │   ├── card_name-description.md          
    │   ├── card_name-solution.md         
    │   ├── order.txt         
    │   └── ...
    ├── C++17                   
    │   ├── card_name-description.md          
    │   ├── card_name-solution.md         
    │   ├── order.txt         
    │   └── ...             
    └── ...

To add a new card:
 
  * Choose a C++ version like **C++20** and add 2 files to the subdirectory.
    * **card_name-description.md** 
    * **card_name-solution.md**
  * Required content of card_name-description.md
    * Headline (# Lambda)
    * Short and pregnant description/instruction
  * Required content of card_name-solution.md
    * Headline (# Solution)
        * Show the solution as code 
    * Headline (# Links)
        * Add a link to cppreference.com
 
After we accept your pull request we will add the card to the order.txt
