# Liste des commandes

## Rails

### Création d'une nouvelle page

Pour cela il faut 3 choses :

- 1 route
- 1 controller avec 1 action
- 1 vue

#### Route

Elle permet à l'application de faire correspondre une URL http://nom_de_domaine/controller/action et 1 controller et 1 action

Dans le fichier `routes.rb` on va définir une route :

```
Rails.application.routes.draw do
...
    get 'contact' => 'contacts#index'
...
```

Ici on va faire correspondre l'URL `http://nom_de_domaine/contact` pour être géré par le controller `ContactsController` et l'action `index`

Il existe de type `get` et `post` :

- `get` permet d'afficher une page (ex.: affichage d'un formulaire)
- `post` permet d'envoyer des informations à une page (ex.: traitement d'un formulaire)
