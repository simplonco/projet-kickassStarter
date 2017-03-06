# projet-kickassStarter
Projet KickAss Starter - 10 jours

## Brief

La start up KickAssStarter souhaite développer une plateforme de Crowed funding. Elle souhaiterait qu’on lui présente un prototype fonctionnel.

## Features

Le site doit comprendre les éléments suivants :

### une page "home public" :

* Un champ de recherche par nom de projet
* une liste de projets (liste de projets par défaut OU résultat de la recherche) 
  * Pour chaque projet :
    * nom
    * description
    * image
    * bouton “Voir”
* un bouton SignIn / SignUp permettant d'ouvrir la modale correspondante

### Modale “Signin” :

* champ texte “email”
* champ text “password”
* bouton "valid"
```
En cas de succès du login, l'utilisateur est redirigé vers la home connectée
```

### Modal “Signup” :

* champ texte “nom”
* champ texte “prénom”
* champ texte “email”
* champ texte “password”
* champ texte “confirm password”
* bouton "valid"
```
En cas de succès du login, l'utilisateur est redirigé vers la home connectée
```

### une page “home connecté” :
* Un champ de recherche par nom de projet
* une liste de projets (liste de projets par défaut OU résultat de la recherche) 
  * Pour chaque projet :
    * nom
    * description
    * image
    * nombre total de likes
    * VALEUR TOTALE DES CONTRIBUTIONS ACTUELLES : XX XXX €
    * bouton “Voir” : redirige vers la page du projet
    * bouton "like" : ajoute un like sur le projet
    
### un menu connecté (pour toutes les pages connectée) :
* un bouton “mes projets” : => vers page “mes projets”
* un bouton “mon compte” : => vers page “compte utilisateur”
* un bouton “créer un projet” : => vers page “Edition / Création de projet”
* un bouton SignOut : => deconnecte la session utilsateur et redirige vers la home public

### Un page “projet”
* nom
* description
* image
* nombre total de likes
* VALEUR TOTALE DES CONTRIBUTIONS ACTUELLES : XX XXX €
* liste des 10 meilleurs contributeurs avec pour chacun la valeur de sa contribution [Seulement présent en mode connecté]
* Champ Number “contribution” : valeur de la contribution €
* bouton “Contribute” OU "Edit my contribution" dans le cas où une contrib a dejà été faite par l'utilisateur : => envoie la valeur saisi dans “contribution” au server
* bouton “edit” [seulement présent si le projet appartient au contributeur] => la page Edition/Création de projet

### Une page “mes projets” :
* liste de mes projets (ceux que j’ai créés)
  * pour chaque projet :
    * nom
    * description
    * image
    * nombre total de likes
    * VALEUR TOTALE DES CONTRIBUTIONS ACTUELLES : XX XXX €
    * nombre total de likes
    * bouton “edit”

### Une page “Edition / Création de projet” :

```
NB : quand on est en mode "création", le formulaire est vide.
``` 

* champ texte nom
* champ texte description
* champ texte image
* nombre total de likes
* liste des contributeurs (avec pour chacun la valeur de sa contribution)
* VALEUR TOTALE DES CONTRIBUTIONS ACTUELLES : XX XXX €
* bouton “validate” (valide la creation ou l’edition et envoie les données au server)
* bouton “delete” [seulement présent en mode édition]

```
NB : Attention : quand on supprime un projet, il faut supprimer ou desactiver les contributions  et les likes utilisateurs liés.
``` 

### Une page "compte utilisateur"

* Nom / Prénom
* Liste des contributions de l'utilisateur
* Liste des likes de l'utilisateur
* bouton "Modifier vos coordonnées" : => vers la page “Edition de compte utilisateur”
* bouton “reset password” : => ouvre une modale "reset password"

### Une page “Edition de compte utilisateur” :
* champ texte “nom”
* champ texte “prénom”
* bouton “validate” (valide la modification et envoie au server)

### Une modale "reset password" :
* champ "old password"
* champ "new password"
* champ "confirm new password"
* bouton “validate” (valide la modification et envoie au server)



