UML README 🚀
# Exo 1 ♦️♥️♣️♠️
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

# Exo 2 ☎️

Notre Diagramme de class est composé de 5 class:

- Client : Qui est en association avec "Call Center"

- Call Center : Qui est en association avec la liste des Employés "Employees". La fonction "SearchEmployee()" cherche dans un employé dans un ordre de priorité, elle fera appelle aux fonctions "IfUnAvailableGoManager()","IfUnAvailableGoDirector()" ainsi que  "IfUnAvailableVoiceMail()" si aucun employé est disponible qui renverra le client vers la boite vocale .

- Employees : Nous permet d'accepter l'appel "AnswerTheCall()" en fonction du status de priorité "StatusPriority"

- Respondent : Nous permet d'executer la fonction "IfUnAvailableGoManager()" dans le cas où le "Respondent" n'est pas disponible (Available : false). "Respondent" hérite de la class "Employees"

- Manager : Nous permet d'excuter la fonction "IfUnAvailableGoDirector()" dans le cas où le "Manager" n'est pas disponible (Available : false). "Manager" hérite de la class "Employees"

- Director : Nous permet d'excuter la fonction "IfUnAvailableVoiceMail()" dans le cas où le "Director" n'est pas disponible (Available : false) . "Director" hérite de la class "Employees"

![Screenshot](Images/CallCenter.png)

# Exo 3 🎼

Notre Diagramme de class est composé de 5 class :

- Person : Nous permet de renseigner les informations importantes "Nom" et "Age"

- Player : Hérite de la class "Person", cette class exécute la fonction "AddACoin()" 

- JukeBox : Qui est en association avec "Player" ainsi qu'avec la liste "Songs", La class "Jukebox" controle la présence d'une pièce de monnaie avec "CoinDetected()" et nous permet de visualiser la playlist avec la fonction "Playlist()" 

- Songs : La class "Songs" est en association avec la class "Author", la class "Songs" nous permet de mettre pause à la chanson avec "Pause()" ainsi que de mettre fin à la diffusion avec la fonction "Stop()"

- Author : Hérite de la class "Person"

![Screenshot](Images/JukeBox.png)


# Exo 04 🚘 

Notre diagramme de class est composé de 5 class : 

Place : qui est caractérisé par sa dimension, sa disponibilité et un ID, et qui représente une place Parking.
Employee: elle representé le personnel employé dans le parking comme la sécurité ou autre.

Barrer : qui joue le rôle du système de barrière à l'entré qui distribue les tickets au clients à l'aide de ses méthodes.

Client : représente un client voulant accèder au parking.

Parking : est la class central qui permet d'articuler l'ensemble des fonctions (acceuillir, les clients, gérer les employés, gérer la disponibilité des places ou gérer le système de barrière) du parking grâce à ses association avec les différentes class.

![Screenshot](Images/Parking.png)


# Exo 05 📚

Notre diagramme de class est composé de 4 class : 

- User qui permet à l'utisateur d'envoyé un message et qui possède un ID pour pouvoir l'authentifier ainsi qu'un username.

- Message qui correspond au message envoyé par l'user et qui possède donc un Propriétaire un destinaire et un corps.

- Postman est la classe qui permet de faire l'intermédiaire entre l'user et le server. 

- Server est une class qui recois une requête (un message) et qui renvoie une réponse adéquate. 

Nous avons utiliser un singleton pour la class Server puisque que nous souhaitons pas avoir plusieurs instance de Server mais récuperer plutot l'instance déjà effective grâce à la méthode getInstance().

![Screenshot](Images/book.png)

# Exo 06 🧩

Notre diagramme de class est composé de 3 class : 

- User : La class permet à l'utilisateur de commencer la partie "Start()" et de recommencer la partie "retry()".

- Jigsaw : La class nous permet de selectionner une piéce "PickPiece(Piece)" de retirer une piéce "RemovePiece(Piece)", "SetPieceOnJigSaw(Piece)" est la méthode qui permet de placer une pièce du puzzle et "CreateJigSaw()" initie le puzzle, La class Jigsaw est composée de la liste "Piece"

- Piece : Qui est caractérisée par un ID et un emplacement au sein du puzzle, est un composant de Jigsaw


![Screenshot](Images/Jigsaw.png)


# Exo 07 ✉️

Notre diagramme de class est composé de 4 class : 

- User qui permet à l'utisateur d'envoyé un message et qui possède un ID pour pouvoir l'authentifier ainsi qu'un username.
- Message qui correspond au message envoyé par l'user et qui possède donc un Propriétaire un destinaire et un corps.
- Postman est la classe qui permet de faire l'intermédiaire entre l'user et le server. 
- Server est une class qui recois une requête (un message) et qui renvoie une réponse adéquate. 

Nous avons utiliser un singleton pour la class Server puisque que nous souhaitons pas avoir plusieurs instance de Server mais récuperer plutot l'instance déjà effective grâce à la méthode getInstance().

![Screenshot](Images/Server.png)



# Exo 08 ♟

Notre diagramme de class est composé de 4 class : 

- Player qui permet à un user d'avoir un nom et de choisir un couleur (Noir ou Blanc)

- Piece qui correspond simplement à aux pièces utilisées lors d'une partie de Othello

- Board qui est composé d'un tableau à 2 dimensions de pièces afin de représenter un tableau d'Othello. Ses fonctions CheckMove(x,y) seront éxecuté lorsque l'user utilisera la fonction Play(x,y). Et il pourra afficher le tableau de la partie en cours.

- Othello Game est la class qui met en place la partie possèdant le nécessaire pour une partie d'Othello c'est à dire : des joueurs (Player) et un tableau composé de Piece (Board et Piece).

![Screenshot](Images/Othello.png)


## Merci Bonne Journée 👐
