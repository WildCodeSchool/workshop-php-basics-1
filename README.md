# PHP BASICS 1

Arrêtez de prendre Salamèche en premier Pokemon. En plus, "bulbe" est le mot le plus sympa à prononcer.
{: .alert-info}

## Démarrage
1.  Crée un dossier `basics`. Dans ce dossier, créé un fichier nommé `index.php`
2.  Lance le fichier PHP directement en CLI (Command Line Interface). Rappel : La commande `php` interprète directement le script
3.  Affiche le message `"Hello Bulbi"`

## Variables

Déclare des variables dans ton fichier `index.php` afin d'y mettre ces données (attention au nommage des variables !)

Si tu souhaites sauter des lignes en PHP, voici un [indice](https://www.delftstack.com/fr/howto/php/php-echo-line-break/).
{: .alert-info }

1.  Ton nom de dresseur, puis affiche le (`string`)
2.  Le nom de ton premier Pokemon, puis affiche le (`string`)
3.  Le niveau de ton premier Pokemon (`integer`)
4.  Si ton Pokemon est KO ou pas (`boolean`)
5.  Renomme ton premier Pokemon, puis affiche le à nouveau (`string`)
6.  Ton Pokemon a bien combattu, il vient de gagner 1 niveau, ajoute le à ta précédente variable (voir les opérateurs arithmétiques), et affiche son nouveau niveau
7.  Affiche la variable `$hometown` (qui n'existe pas) et observe le message d'erreur
8.  Initialise la variable `$hometown` avec le nom de ta ville d'origine avant de l'afficher.  
    Magie, l'erreur a disparu !  
![](surprised-pikachu.jpg)

## Strings

1.  Affiche la phrase suivante : "Je m'appelle _TRAINER_NAME_" (remplacer par la variable déclarée précedemment)
2.  Affiche la phrase suivante : "mon premier Pokemon est _FIRST_POKEMON_NAME_. Où est la première arène svp ?" (remplacer par la variable déclarée précedemment)
3.  Concatène ces deux phrases en y ajoutant le mot de liaison "et" _(Ex: Je m'appelle Mickaël et mon premier Pokemon est Bulbizarre. Où est la première arène svp ?)_

## Include / Require

Nous allons quitter le mode CLI (ne supprime pas ton travail effectué jusque là) pour afficher nos résultats via le navigateur. Pour cela, démarre un serveur HTTP sur le dossier `basics` et ouvre le fichier `index.php` dans ton navigateur préféré.
{: .alert-warning}

1.  Crée un fichier `header.php` affichant la phrase "Bienvenue au centre Pokemon, comment vous appelez vous ?".
2.  Crée un fichier `footer.php` affichant la phrase "Merci, bonne journée !".
3.  Utilise `include` dans ton fichier `index.php` afin d'afficher le header et le footer respectivement au début et à la fin de ton fichier.
4.  Juste avant celui du footer, fais un include du fichier `arena.php` **sans créer le fichier**. Puis utilise `require` au lieu d'`include` afin d'observer la différence.
5.  Crée le fichier `arena.php` affichant la phrase "C'est un peu tôt pour vous le dire". Le texte doit apparaître désormais.
6.  Remplace ta phrase dans le fichier `arena.php` par : `echo $firstArena;`. Il y a une erreur et c'est normal, la variable n'existe pas encore.
7.  Afin d'y remédier, dans `index.php` créé une variable `$firstArena = 'Argenta';` **AVANT** d'include/require le fichier `arena.php`, tu ne dois plus avoir d'erreur, et avoir une conversation qui tient la route.


![](https://media.giphy.com/media/xuXzcHMkuwvf2/giphy.gif)