﻿# Utilisation de l'API JSONPlaceholder avec Postman

## 1. Requête GET sur les `comments`

### Étapes :

1. Ouvrez Postman.
2. Créez une nouvelle requête.
3. Sélectionnez `GET` comme méthode.
4. Entrez l'URL : `https://jsonplaceholder.typicode.com/comments`.
5. Cliquez sur `Send`.

### Résultat :

Vous obtiendrez une liste de tous les commentaires disponibles dans la base de données.

---

## 2. Requête POST sur les `todos`

### Étapes :

1. Créez une nouvelle requête.
2. Sélectionnez `POST` comme méthode.
3. Entrez l'URL : `https://jsonplaceholder.typicode.com/todos`.
4. Dans l'onglet `Body`, sélectionnez `x-www-form-urlencoded`.
5. Ajoutez les paramètres suivants (exemple) :
   - `userId`: `1`
   - `title`: `My new todo`
   - `completed`: `false`
6. Cliquez sur `Send`.

### Résultat :

Une réponse contenant l'objet créé (avec un nouvel identifiant) sera renvoyée.

---

## 3. Requête PATCH sur les `posts`

### Étapes :

1. Créez une nouvelle requête.
2. Sélectionnez `PATCH` comme méthode.
3. Entrez l'URL : `https://jsonplaceholder.typicode.com/posts/1` (remplacez `1` par l'identifiant d'un post existant).
4. Dans l'onglet `Body`, sélectionnez `raw` et choisissez le type `JSON`.
5. Entrez le contenu suivant pour modifier le `title` et le `body` :
   ```json
   {
     "title": "Updated Title",
     "body": "This is the updated body"
   }
   ```
6. Cliquez sur `Send`.

### Résultat :

Un objet post mis à jour avec les nouvelles valeurs.

---

## 4. Requête GET pour afficher les commentaire du`post`avec id=`1`

### Étapes :

1. Créer une nouvelle requête.
2. Sélectionnez `GET` comme méthode.
3. Entrez l'URL : `https://jsonplaceholder.typicode.com/posts/1/comments`.
4. Cliquez sur `Send`.

### Résultat :

Une liste des commentaires associés au post ayant l'identifiant `1`.

---

## 5. Requête GET pour afficher les photos de l'`album`avec numero `2`

### Étapes :

1. Créer une nouvelle requête.
2. Sélectionnez `GET` comme méthode.
3. Entrez l'URL : `https://jsonplaceholder.typicode.com/albums/2/photos`.
4. Cliquez sur `Send`.

### Résultat :

Une liste des commentaires associés au post ayant l'identifiant `2`.

## Notes

### Étapes :

1. Ces requêtes utilisent l'API JSONPlaceholder, qui ne nécessite pas d'authentification.
2. L'API est conçue pour les tests et renvoie des réponses simulées.
