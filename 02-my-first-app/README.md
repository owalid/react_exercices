```
npx create-react-app my-first-app
cd my-first-app
npm start
```

# Introduction

- Familiariser vous avec le code, tentez de changer du texte dans le code et de voir ce qui se passe. etc.
- Crée un nouveau composant que l'on va appeler `HelloWorld` dans le fichier `HelloWorld.js` et qui va retourner un élément h1 avec le texte "Hello World".

# Props

- Faite en sorte que le composant `HelloWorld` soit affiché dans le composant `App` en utilisant la balise `<HelloWorld />` dans le composant `App`.
- Ajouter maintenant un props `name` au composant `HelloWorld` et afficher le dans le h1 du composant.

# Hooks (useState)
- Faite en sorte que le message "Hello world" soit modifiable. Ajouter donc un input text dans le composant `HelloWorld`. Afficher le nouveau nom dans le h1 en plus du props. (useState)
- Crée un nouveau composant que l'on nommera `DateNowState` et qui va retourner un élément h1 avec la date d'aujourd'hui.
- Ajouter maintenant un bouton dans le composant `App` qui va permettre de changer la date affichée dans le composant `DateNowState` en utilisant le hook `useState`.

# Hooks (useEffect) sans nettoyage
- Dans le composant `DateNowEffect` ajouter un useEffect qui va afficher la date d'aujourd'hui dans la console.

# Hooks (useEffect)
- Crée un nouveau composant que l'on nommera `DateNowEffect` qui aura le meme principe que le composant `DateNowState` mais sans le bouton. Il faudra donc qu'il affiche la date d'aujourd'hui et qu'il se mette à jour toutes les secondes. en utilisant le hook `useEffect`. Faite en sorte de clean le hook `useEffect` avec `cleanInterval` pour éviter les fuites de mémoire.

# Hooks (personalisé)
- Crée un composant `IncrementBouton` qui aura un hook personalisé qui va permettre d'incrémenter un nombre de 1 en 1 lors du click du boutton. Ce composant va retourner un bouton qui va afficher le nombre incrémenté.

- Crée ensuite un nouveau composant `AutoIncrementButton` qui aura un hook personalisé (`useAutoIncrement`) qui mettra à jours toutes les secondes la valeur count. Ce composant va retourner un bouton qui va afficher le nombre incrémenté. Faite en sorte de clean le hook `useEffect` avec `cleanInterval` pour éviter les fuites de mémoire.

# Hooks (useContext & styles)
- Crée un nouveau contexte `ThemeContext` qui aura un state `theme` qui aura comme valeur par défaut `light`.
- Ce theme sera consomé pour changer la couleur du texte et de background des composants crée juste avant.
- Ajouter un bouton dans le composant `App` qui va permettre de changer le theme entre `light` et `dark` en utilisant le contexte `ThemeContext`.

# Appel d'API

- Crée un nouveau composant appeler `PostsLists` qui va afficher une liste de posts. Récuperer à partir de l'API `https://jsonplaceholder.typicode.com/posts?_limit=5`.
- Ajouter aussi un bouton pour supprimer un post de la liste.
- Vous devez utiliser les hooks que vous avez vu precedement (`useEffect` et `useState`).
- Ajouter un state `loading` qui va permettre d'afficher un message de chargement pendant que les données sont en train d'être chargées.
- Refactorisé le tout pour avoir un hook personalisé que l'on va appelé `useFetch` qui va permettre de faire les appels à l'API et le chargement.

# useCallBack
- Crée un nouveau composant appelé `City`, qui aura deux state, un state `name` et un state `numberOfHabitants`. Ce composant va retourner un h1 avec le nom de la ville et le nombre d'habitants.
- Il faudra aussi ajouter un input number qui va permettre de changer le nombre d'habitants de la ville. Ainsi qu'un input type text qui va permettre de changer le nom de la ville.
- Ajouter un console.log à l'intérieur du composant `City` qui affiche le nombre d'habitants pour voir combien de fois il est appelé.
- Déplacer le console.log pour faire en sorte qu'il soit appeler uniquement lorsque le nombre d'habitants change.
- Il faudra utiliser le hook `useCallback` pour éviter que la fonction `console.log` soit appelé à chaque fois que le composant `City` soit rerender.

# Memo
- Crée un nouveau composant appelé `ButtonMemo` qui auras un console.log à la création du composant. Ce composant va retourner un bouton qui va afficher le nombre de fois qu'il a été cliqué.
- Ajouter ce composant au composant `IncrementButton`
- Observer le nombre de fois que le composant `ButtonMemo` est appelé dans la console. Lorsque le boutton du composant `IncrementButton` est cliqué.
- Ajouter un `React.memo` au composant `ButtonMemo` pour éviter que le composant ne soit appelé à chaque fois que le composant `App` est appelé.
- Observer le nombre de fois que le composant `ButtonMemo` est appelé dans la console.
