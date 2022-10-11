```
npx create-react-app .
npm start
```

- Maintenant que vous êtes familier avec le code, nous allons construire notre premiere app react. En implementant etape par etape une application de liste de taches (todo app). Nous allons voir les principes suivants: Events, Formulaire, state, props, events, lifecycle, etc.


# Composants

- TodoForm est un composant qui va afficher un formulaire avec un input et un boutton. Il va aussi gerer les evenements du formulaire et les soumissions.
- Le composant Task est une tache aura un etat de fait ou non fait ainsi qu'une description. Il faudra donc ajouter un boutton pour changer l'etat de la tache. Le fait de passer de passer la tache en fait ou non fait va changer la couleur de la tache dans la liste. Il faudra aussi ajouter un boutton pour supprimer la tache ansi qu'un boutton pour modifier la tache.
- TodoList est un composant qui va afficher une liste de Task. Il va recevoir une liste de todo en props et va les afficher dans une liste ul. Chaque todo sera affiché dans une balise li. Pour chaque todo, il va afficher le texte du todo et un boutton pour supprimer le todo.

# Events

- 