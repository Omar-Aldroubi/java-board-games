Groupe n° 001 :

Khalil Mohammad 

Mohamad Omar Aldroubi 


Le dossier src/ contient les fichier .java organisé dans des packages comme demandés.

Les classes exécutables sont :

package games.nim :
	- games.nim.DemoNim : permet de jouer une partie de Nim à 2 joueurs 
	- games.nim.TestNim : lance les tests unitaires sur la classe Nim

package games.tictactoe
	- games.tictactoe.DemoTicTacToe : permet de même de jouer 
	  au jeu de morpion   	   
	- games.tictactoe.TestTicTacToe : lance les tests unitaires
	  sur la classe TicTacToe 

package games.factoredgames :
	- games.factoredgames.DemoNim : version optimisé du jeu de nim

	- games.factoredgames.DemoTicTacToe : version optimisé du jeu de morpion

	- games.factoredgames.TestAbstractGame : lance les tests sur 
	  la classe  AbstractGame
	
	- games.factoredgames.TestNimEtTicTacToe : lance les tests
	  sur les classes Nim et TicTacToe 
	- games.factoredgames.TestTicTacToeWithHints : lance les tests
	  sur la classe TicTacToeWithHints

package games.genericgames :
	- games.genericgames.DemoNim
	- games.genericgames.DemoTicTacToe
	- games.genericgames.TestGenericGames : lance les tests sur les 
	  classes du package
	  
package games.player : 
	- games.player.TestPlayer : lance les tests sur les classes du package


package games.plays :
	- games.plays.Main : classe principal du projet qui les utilise toutes
	les classes et interfaces
	- games.plays.TestPlays : lance les tests sur les classes de plays
	
Remarques :
- tous les tests ont été passés sauf un(HumanTests dans
  games.players.TestPlayers)
  on l'a commenté pour voir les tests d'après
    
- TicTacToeWithHints n'est pas implementé dans genericgames
  
  
pour lancer un programme principal, placez vouz dans src et lancez les commandes suivants:
REMARQUE: ici on suppose que il existe un repertoire lib qui contien bibliothèques des tests (fichiers .jar)

- Compiler: javac -d .:../build -cp ../lib/gamestest.jar games/plays/*.java

- lancer le jeu: java -cp ../build:../bib/gamestests.jar games.plays.Main  

Une javadoc a été réalisée, mais seulement les classes ont été documentées.















