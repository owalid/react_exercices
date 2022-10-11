```
npx create-react-app .
npm start
```

# Introduction

- Familiariser vous avec le code, tentez de changer du texte dans le code et de voir ce qui se passe. etc.
- Crée un nouveau composant que l'on va appeler `HelloWorld` dans le fichier `HelloWorld.js` et qui va retourner un élément h1 avec le texte "Hello World".

# Props

- Faite en sorte que le composant `HelloWorld` soit affiché dans le composant `App` en utilisant la balise `<HelloWorld />` dans le composant `App`.
- Ajouter maintenant un props `name` au composant `HelloWorld` et afficher le dans le h1.

# Events

- Ajouter maintenant un boutton dans le composant `HelloWorld` qui va uniquement afficher dans la console "Hello World" quand on clique dessus.

# Hooks

- Changer l'evenement du boutton pour qu'il change le texte du h1 en "Hello World" + nom quand on clique dessus. (Cela sous entend que le texte du h1 doit etre dans le state du composant) (useState)
- Faites en sorte d'initialiser le state du composant avec le props `name` (useEffect).
- A chaque fois que le state change, afficher dans la console le nouveau state (useEffect).
