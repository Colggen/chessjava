Firstly, I want to tell about right input of the project. I have created chess game, so to take a move you should write it like "a2-a4" for each figure.
To do castling you should write "0-0 wh" - for short castling and "0-0-0 wh" for long castling in white figures case; and "0-0 bl" , "0-0-0 bl" for black figures.

1. The Reuse/Release Equivalence Principle
I have divided my files by reusability and by cohesion. Because I can't have each figure in different package, for example if I will have Bishop
in another package, and I want to add game 2x2 I should change all code in another components.

2. The Common Closure Principle.
As this principle is closed to Open-Closed principle, I have divided classes by components, to avoid changing the code of others components.
So if I changed one class it will be better to change only one component, the others.
It means that in our project we should minimize number of packages that are changed for any release.

3.The Common Reuse Principle.
I have separated components according to their responsibilities. It means that each component have their own responsibility.
For adding dependency, every class of the component should be used. For example if I use DrawBoard package, I use all the files in the GameLaunch package.
