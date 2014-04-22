#Planet Wars Bot#

In this practice we are going to start using Planet Wars. Just a few
notes are given here. The rest can be consulted at the webpage of Planet
Wars Competition:

[http://planetwars.aichallenge.org/index.php](http://planetwars.aichallenge.org/index.php)

Where starting instructions can be found, along with some advices and
tutorials on how to create your bot.


##WHAT TO DO##

1.  Download the framework (source files, examples, tools, maps) from:

[http://geneura.ugr.es/\~amorag/courses/eas\_in\_games/materials/PLANETWARS.zip](http://geneura.ugr.es/~amorag/courses/eas_in_games/materials/PLANETWARS.zip)


or clone this repository:


[https://github.com/deantares/botPlanetWars](https://github.com/deantares/botPlanetWars)



​2. Unzip it wherever you want.

​3. You will have the following directories:

​* example\_bots  some examples to test your own bot

​* maps  a list of 100 maps to test your bot

​* maps\_images  png files showing the maps appearance

​* tools  Game Player and Game Visualizer

##WHERE TO IMPLEMENT AI:##

​4. You just have to change the function DoTurn() included in
MyBot.java.

​5. You can access pw object, which contains the game information and
functionalities.

​6. The method IssueOrder is in charge of performing an order (actions)
in the game.

##COMPILE A BOT:##

​7) Just write inside the folder where your bot is (and also the files
PlanetWars.java, Planet.java, and Fleet.java):

`Javac \*.java`

RUN A GAME

​8. Once you have defined your bot and compiled it, you can make a
combat (and show) between it and another bot with the command:

`java –jar \<path\_tools\>/PlayGame-1.2.jar \<map.txt\> \<time\_ms\>
\<num\_turns\_max\> \<log\_file\> “java \<path\_MyBot\>/MyBot” “java
–jar \<path\_OtherBot\>/bot2.jar” | java -jar tools/ShowGame-1.2.jar`

Or (if you will use a jar file for your bot):

`java –jar \<path\_tools\>/PlayGame-1.2.jar \<map.txt\> \<time\_ms\>
\<num\_turns\_max\> \<log\_file\> “java –jar \<path\_MyBot\>/MyBot.jar”
“java –jar \<path\_OtherBot\>/bot2.jar” | java -jar
tools/ShowGame-1.2.jar`

​9. If, for instance, you generate a jar file with your bot and just
want to do the battle with no visualization, you can use the command:

`java –jar \<path\_tools\>/PlayGame-1.2.jar \<map.txt\> \<time\_ms\>
\<num\_turns\_max\> \<log\_file\> “java –jar \<path\_MyBot\>/MyBot.jar”
“java –jar \<path\_OtherBot\>/bot2.jar”`


***\* Note: Do not copy-paste the commands, since there could be
problems with the characters***
