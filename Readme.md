# Monsters and Heros
This is a text-based role playing game game built in Java, where the player controls a party of heroes who fight monsters and gain experience and money. The game is played on a fixed, square grid of spaces containing inaccessible spaces, market spaces, and common spaces. The player moves the party of heroes to adjacent spaces and can enter the market if the party is on a market space.

## Installation
To run this game, you must have Java installed on your computer. Clone this repository to your local machine, and navigate to the directory where the repository is located in your terminal or command prompt. Then, run the following command:
javac *.java

This will compile all of the Java files. To start the game, run the following command:
java GameEngine

## How to Play
When you start the game, you will be prompted to choose how many heroes you want in your party. Once you have chosen, the game will generate a map with a fixed, square grid of spaces containing inaccessible spaces, market spaces, and common spaces.

To move the party of heroes, type the direction you want to move (up, down, left, or right) and press enter. If the party is on a market space, you can enter the market by typing "market" and pressing enter.

Every time the heroes visit a common tile, there is a chance that they will engage in a battle with the monsters. During the battle, the player chooses for each hero whether they will attack, cast a spell, use a potion from the hero’s inventory, or equip a weapon or piece of armor from the hero’s inventory. The monsters’ turn begins after the heroes have made their moves. The monsters will only attack the heroes, as they do not have items or spells to use.

The game ends if all of the heroes have fainted or if the player decides to quit. If the heroes defeat all of the monsters, they gain experience and money, potentially leveling up. If a hero faints, they are revived with half of their HP and mana, but they will not gain any gold or experience.

## Code Structure
1. Armor.java: This is the class which has functions and attributes related to all types of Armors.
2. Battle.java: This class hold everything that happens during a battle.
3. Board.java: This is the super Board class. This class has attributes and functions which are common to all possible game boards.
4. BoardCells.java: This class has attributes and functions which has to be implemented on a specific board cell.
5. Consumable.java: Super class for Spells and Potion. This class has functionalities common to both of them.
6. ConsumableFactory.java: Instance generator factory for Consumable type items
7. Dragon.java: This class implements the monster interface. Dragons are a type of monsters and this class holds all the functionalities specific to Dragons
8. Equipable.java: Super class for Armor and Weapon. This class has functionalities common to both of them
9. Equipable.java: Instance generator factory for Equipable type items
10. Exoskeletons.java: This class implements the monster interface. Exoskeletons are a type of monsters and this class holds all the functionalities specific to Exoskeletons
11. FireSpells.java: This class implements the Spells interface. This class hold all the functionalities related to specific spell items called Fire spells
12. Game.java: This is the interface which all the game classes implements. It has the common functionalities of all the games
13. GameEngine.java: This is the main class which will call the specific game class. This class can have instances of different game classes.
14. GridBoard.java: This is the class for all Grid type boards like chess board, tic-tac-toe board. It has all the attributes and functions for Grid type board
15. Hero.java: This is the interface which has signatures of functions common to all Heroes
16. HeroFactory.java: Instance generator factory for Heroes typed Roles
17. IceSpells.java: This class implements the Spells interface. This class hold all the functionalities related to specific spell items called Ice spells
18. ItemFactory.java: This is the super class of specific instance generator classes of type Item
19. Items.java: This is the interface which has functionalities common to all Items
20. ItemsFactoryProducer.java: This class produces factories specific to required Item type
21. Legends.java: This is the class for the Legends game. It has all the attributes and methods related to Legends game.
22. LighteningSpells.java: This class implements the Spells interface. This class hold all the functionalities related to specific spell items called Lightening spells
23. Market.java: This class handles all the functionalities related to the Market
24. Monster.java: This is the interface which has signatures of functions common to all Monster
25. MonsterFactory.java: Instance generator factory for Monsters typed Roles
26. Paladin.java: This class has functions and attributes related to all Paladin typed Heroes and this class also implements the hero interface
27. Potions.java: This is the class which has functions and attributes related to all types of Potions
28. RolePlayingGame.java: This class has functions and attributes common to all Role Playing games
29. Roles.java: This interface has all the functionalities common to all roles
30. Sorcerer.java: This class has functions and attributes related to all Sorcerer typed Heroes and this class also implements the hero interface
31. Spells.java: This is the interface which has functionalities common to all Spells
32. Spirits.java: This class implements the monster interface. Spirits are a type of monsters and this class holds all the functionalities specific to Spirits
33. Warrior.java: This class has functions and attributes related to all Paladin typed Heroes and this class also implements the hero interface
34. Weapon.java: This is the class which has functions and attributes related to all types of Potions

## Future Improvements
This game can be improved in many ways, such as adding more types of monsters, weapons, and spells, allowing the player to customize the heroes' attributes and skills, and implementing a more complex battle system. Additionally, the game can be made more visually appealing by using graphics and sound effects.