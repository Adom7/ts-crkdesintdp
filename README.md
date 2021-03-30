UML README 🚀

Notre diagramme de class est composé de 5 class : 
- Card : Qui utilise des enumération : 
    - CardSymbols : Qui correspond au différents symboles que la "Card" peut avoir
    - Number : Qui correspond au différentes valeurs que la "Card" que la carte peut avoir

- Deck : Qui est composé de plusieurs "Card"
- BlackJack : Qui est en association avec "Deck" , "Player" et "Dealer"
- Player : Qui effectue les opérations demandées
- Dealer : Qui effectue les opérations demandées

La Class "BlackJack" est la class principale, "BlackJack" utilise les autre class pour mettre en oeuvre le jeu

![Screenshot](images/DeckOfCard.png)