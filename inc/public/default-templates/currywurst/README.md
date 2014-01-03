# Currywurst

Un nouveau jeu de templates par défaut pour Dotclear (versions ≥ 2.7)

## Motivations

Le jeu de templates Currywurst répond à divers objectifs :

- Proposer un jeu de templates en HTML 5.
- Pouvoir ainsi y introduire des balises [http://fr.wikipedia.org/wiki/Accessible_Rich_Internet_Applications](ARIA) pour une meilleure accessibilité.
- Améliorer la sémantique des tags html (par exemple ne plus présenter les commentaires dans une liste de définition).
- Factoriser les éléments récurrents dès que c'est possible sans pâtir à la compréhension.
- Préparer le passage à la syntaxe [http://twig.sensiolabs.org/](twig).
- Adopter une nomenclature inspirée de [http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/](BEM) – sans en faire une religion dogmatique toutefois. Voir aussi [http://coding.smashingmagazine.com/2011/12/12/an-introduction-to-object-oriented-css-oocss/](OOCSS).
- Faire en sorte de réduire l'obligation de recourir aux sélecteurs enfants (`#top h1 {}` par exemple) ou aux ID dans les CSS.

## Revue fichier par fichier

Ne sont pas listées les modifications systématiques : ajout de classes sur tous les éléments « probablement stylés » ou ne possédant qu'un id ; syntaxe html5.

Les modifications nécessitant des explications sont listées de la façon suivante :

    <Description courte> : <motivation>. <Explication>.

Les motivations sont abrégées en :
- a11y : amélioration accessibilité
- sém. : amélioration ou correction sémantique (html)
- cont. : amélioration du contenu
- ergo : amélioration ergonomique

Par convention l'ordre des attributs dans les balises html est *class, id, autres attributs*.

### _top.html

Déplacement des liens d'accès rapides au-dessus du titre du blog : **a11y**, **ergo**. *Le titre de fenêtre étant lu avant tout par les aides techniques, l'internaute sait déjà où il se trouve. L'accès est également plus rapide au clavier. Côté design, la plupart des créateurs de thèmes ont pris l'habitude de déplacer ce bloc en haut de la page ; ils n'auront plus besoin de passer par des position absolute pour ce faire.*
