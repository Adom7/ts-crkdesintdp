UML README 🚀
# Exo 1
Notre diagramme de class est composé de 5 class : 
- Card : Qui utilise des enumération : 

    - CardSymbols : Qui correspond au différents symboles que la "Card" peut avoir
    - Number : Qui correspond au différentes valeurs que la "Card" que la carte peut avoir

- Deck : Qui est composé de plusieurs "Card"

- GameCard : Nous permet de créer un jeu de carte universel (des regles partagées par tout les jeux de cartes) Game Card est en association avec "Player" ainsi que "Deck"
Puisque GameCard est une class abstraite, GetCardValue sera à redéfinir pour chaque dans chaque class fille afin d'attribuer la valeur pour chaque card du Deck

- BlackJack : Qui est en association avec "Dealer" et hérite de "GameCard"

- Player : Qui effectue les opérations demandées

- Dealer : Qui effectue les opérations demandées

La Class "GameCard" est la class principale, en héritant de "GameCard" , "BlackJack" utilise les autres class pour mettre en oeuvre le jeu.

![Screenshot](Images/DeckofCards.png)

# Exo 2

Notre Diagramme de class est composé de 5 class:

- Client : Qui est en association avec "Call Center"
- Call Center : Qui est en association avec la liste des Employés "Employees"