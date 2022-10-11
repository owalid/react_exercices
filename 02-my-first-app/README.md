```
npx create-react-app myfirstapp
cd myfirstapp
npm start
```

# Introduction

- Familiariser vous avec le code, tentez de changer du texte dans le code et de voir ce qui se passe. etc.
- Crée un nouveau composant que l'on va appeler `HelloWorld` dans le fichier `HelloWorld.js` et qui va retourner un élément h1 avec le texte "Hello World".

# Props

- Faite en sorte que le composant `HelloWorld` soit affiché dans le composant `App` en utilisant la balise `<HelloWorld />` dans le composant `App`.
- Ajouter maintenant un props `name` au composant `HelloWorld` et afficher le dans le h1 du composant.

# Events and Hooks

- Faite en sorte que le message "Hello world" soit modifiable. Ajouter donc un input text dans le composant `HelloWorld`. Afficher le nouveau nom dans le h1 en plus du props. (useState)
- Dans le composant `App`, changer la valeur qui est passer dans le composant `HelloWorld` (le props `name`) pour qu'il soit maintenant dynamique. (useState)
- Ajouter ensuite dans le compsant App une fonction qui va prendre en paramètre un nouveau nom et qui va changer le state du composant `App`. La nouvelle valeur sera la concatenation du parametre de la fonction (name) avec 'and me' (`name + 'and me'`) (useState)
- Ajouter un nouveau props au composant `HelloWorld` qui sera la fonction que vous venez de crée.
- Ajouter ensuite un nouvel input text dans le composant `App` et un boutton. Au clique du boutton il devra appeler la fonction qui sera passer en props avec la valeur de l'input (e.target.value). (pensez au `e.preventDefault()`)


# Map

- Crée un nouveau composant `List` qui aura un state qui sera un tableau de string. (useState)
- Dans ce composant `List` afficher le tableau de string dans une liste ul li. (pensez à utiliser la fonction map et à passer une `key` en props de chaque élément de la liste)
- Ajouter un input text et un boutton dans le composant List qui permettra d'ajouter une nouvelle string dans le tableau. (penser à utiliser un useState pour l'input text)
- Importer ensuite le composant dans le composant `App` et afficher le.
