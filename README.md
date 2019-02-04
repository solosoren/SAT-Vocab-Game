# SAT Vocab Game

## About
SAT Vocab Game is a speed typing educational game designed to help learn SAT vocabulary. When the game starts enemy words come down the screen to attack the player. The user must type out the words in order to destroy them. The goal is to survive as long as possible before getting hit. 

There are two game modes: the default mode, and the SAT prep. The default mode is a general list of words that grow in length each round. The SAT prep mode is a list of vocabulary words used in the SAT. 

[App Preview](https://youtu.be/IkJ4Xtj63wU)

## My Contributions
Most of my work was on the Backend. This included the GameObjects and all of its Subclasses, ObjectController, and LoadWords.

#### GameObjects and Subclasses
This is essentially the Model for our app. We created a GameObjects Superclass so we could pass a Vector of GameObjects’ Pointers to the Frontend. This allows the Backend to do any object manipulation and adding/removal of the objects from the Vector. The Frontend then only had to loop through the Vector and display each object. 

#### ObjectController
This class manipulates the objects and contains the Box2D code as well as the game logic. I did most of the object manipulation and game logic.

#### LoadWords
LoadWords is a static class. It was initially used to sort the list of Default Game Mode Words in a .txt file. These words are imported at the beginning of every game. At the beginning of each round, it creates a vector of words to be used. Then every time a word is used it returns the next word in the vector.

## Photos
<img src="https://github.com/solosoren/SAT-Vocab-Game/blob/master/Shooting%20Enemy.png" width="300">
<img src="https://github.com/solosoren/SAT-Vocab-Game/blob/master/End%20Of%20Round%20Stats.png" width="300">

## References

- [zty.pe](https://zty.pe/)
- [Box2D](https://github.com/erincatto/Box2D)
- [SFML](https://www.sfml-dev.org/index.php)
- [Default Game Mode Words](http://www.wordfrequency.info)
