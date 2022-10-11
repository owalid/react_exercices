```
npx create-react-app todoapp
cd todoapp
npm start
```

- Maintenant que vous êtes familier avec le code et l'environement de react, nous allons construire notre premiere (vrai) app react. En implementant etape par etape une application de liste de taches (todo app). Nous allons voir les principes suivants: Events, Formulaire, state, props, lifecycle, etc.

- Créer un nouveau dossier components dans le dossier src et créer un fichier TodoForm.js


- Une tache est un objet avec un id, un titre et un etat (done ou non). Nous allons utiliser un tableau pour stocker les taches. Nous allons utiliser un id unique pour chaque tache. Nous allons utiliser la librairie uuid pour generer des id uniques.

Exemple:
```json
[
  {
    "id": "1",
    "title": "Learn React",
    "done": false
  },
  {
    "id": "2",
    "title": "Learn Redux",
    "done": false
  },
  {
    "id": "3",
    "title": "Learn HTML",
    "done": true
  }
]
```


# Composants

- App.js sera le composant pere de votre site. Il auras pour role de gerer les taches et de les passer en props aux composants enfants. Il auras un state qui contiendra la liste des taches. Il auras aussi une methode qui permettra d'ajouter une tache a la liste.

- AddTodo (components/AddTodo.js) est un composant qui va afficher un formulaire avec un input et un boutton. Il va aussi gerer les evenements du formulaire et les soumissions. Il aura besoin d'un props `addTodo` qui sera une fonction de composant pere qui permettera de mettre à jours la liste des taches.

- Dans le composant App faites en sorte d'afficher les taches dans une liste en utilisant un map.

Pour chaque tache:

  - Afficher le titre.
  - Un boutton qui permettra de supprimer la tache.
  - Un bouton qui permettra de marquer la tache comme faite. Si la tache est marqué comme faite il faudra ajouter un style css qui va barrer le texte. Il faudras aussi changer le texte du boutton pour "Marquer comme non faite" ou "Marquer comme faite" en fonction de l'etat de la tache.
  - Un bouton qui permettra d'editer la tache.

- Au moment ou on clique sur "editer la tache" un nouveau formulaire apparait sous la tache:

- EditTodo (components/EditTodo.js) est un composant qui permettra de modifier une tache. Il aura besoin d'un props `editedTodo` qui sera la tache a editer. Il aura aussi besoin d'un props `changeTitleTodo` qui sera une fonction de composant pere qui permettra de mettre à jours la liste des taches.


# State et methodes

- Dans le composant App vous allez avoir besoin de deux states, un state qui sera la liste des taches et un state qui sera la tache a editer.

Vous allez aussi avoir besoin de plusieurs methodes pour mettre à jours les states:
- Une methode pour mettre à jours une tache
- Une methode pour ajouter une tache
- Une methode pour supprimer une tache

- Dans les composants AddTodo et EditTodo vous allez avoir besoin d'un state qui sera le titre de la tache. (Attention pour le composant EditTodo le state sera initialisé avec le titre de la tache a editer)
Vous allez avoir besoin d'une methode:

- Qui permet de mettre à jours le titre de la tache qui sera appelé a chaque fois que l'utilisateur clique sur le bouton de soumission du formulaire. (penser a verfier si votre titre n'est pas vide)

