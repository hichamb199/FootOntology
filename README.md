L'objectif ici n'était pas de construire des profils d'objectifs mais de montrer qu'il est possible d'apporter une connaissance subjective et de l'appliquer au monde du football.
Nous avons défini plusieurs familles de classes :
- Clubs : ces classes contiennent tous les clubs de football des différents pays européens les championnats nationaux utilisés dans l'ontologie. Ils sont utilisés pour représenter dans quel club les joueurs jouent réellement. Nous avons classé les clubs sur la base d'une une propriété de données appelée APrestige qui représente le prestige du club. 
- Ligues : ces classes contiennent les championnats nationaux dans lesquels les clubs jouent. 
- Joueurs : ces classes contiennent tous les joueurs à classer dans l'ontologie. Les joueurs sont classés selon la position qu'ils occupent sur lequel ce soit en fonction du profil déduit par le raisonneur.
- CaracteristiquesJoueurs : regroupe les Positions(Postes), Profils et PiedsForts pour un affichage plus facile de ces classes. Ce sont les mêmes classes qui sont contenues dans les classes Joueurs puisqu'il s'agit de sous-classes de Joueurs et de CaracteristiquesJoueurs.

Nous avons utilisé les propriétés des objets pour relier les objets entre eux :
-estLigueDe : pour spécifier dans quelle ligue nationale un club joue (JoueDansLeague étant la propriété opposée) 
- JoueDansPoste : pour préciser le rôle des acteurs sur le terrain.
- JoueAvecPied : pour spécifier si le joueur est droitier ou gaucher (estMeilleurPied étant la propriété opposée).
- JoueA : pour spécifier dans quel club un joueur joue effectivement (estClubDe étant la propriété opposée)
Nous avons également utilisé les propriétés des données pour relier les statistiques à leur entité dans l'ontologie :
- APrestige : prestige d'un club sur la scène internationale (entier entre 1 et 5)
- EstAgeDe : âge d'un joueur (entier)
- AUneSelectionNationale : indiquez si le joueur joue dans une équipe nationale ou non, et si oui contient le nombre de sélections (nombre entier entre 0 et 300)
- aUneTailleDe : taille d'un joueur (nombre entier entre 150 et 250 centimètres)
- aUnPoidsDe : poids d'un joueur (entier entre 60 et 120)
- aUnGeneralDe : état général d'un joueur (nombre entier entre 0 et 100)
- aUneTechnique : état technique du joueur (nombre entier entre 0 et 100)
- aUnMentalDe : état mental du joueur (nombre entier entre 0 et 100)
- aUnPhysiqueDe : état physique du joueur (nombre entier entre 0 et 100)

Nous avons également renseigné d’autres caractéristiques générales pour les joueurs :  
Joueur d’impact physique (max(stats)->Physique
Joueur technique (max(stats)->Technique)
Joueur de caractère (max(stats)->Mental)
Top joueur (niveau général > 80)
Attaquant (poste d’attaque)
Milieu de terrain (poste milieu)
Défenseur (poste défenseur)
Joueur d’expérience (age > 28, prestige équipe > 3)
Jeune joueur prometteur (age < 22, niveau général > 75)
Star (niveau général > 90, prestige équipe = 5)

Liste des caractéristiques de profils techniques par postes pour les joueurs 
Grand gardien (Taille > 1,9m, niveau physique/mental > 80, prestige équipe > 3)
Gardien agile ( Taille < 1,9m, niveau technique > 80)
Défenseur central d’expérience (Age > 28, niveau physique/mental > 80, international > 0, prestige d’équipe > 3)
Défenseur central polyvalent (niveau général > 75, niveau technique > 80, peut jouer à plusieurs postes (défenseur central ou latéral))
Latéral polyvalent (peut jouer à droite ou à gauche)
Latéral gauche/droit (joue uniquement à gauche/droite)
Latéral offensif (Niveau physique/technique > 80)
Milieu de terrain technicien (Joueur technique, joue au milieu de terrain)
Milieu de terrain récupérateur (Joueur physique, joue au milieu de terrain)
Sentinelle (Joueur physique, niveau technique > 80, joue au milieu de terrain)
Milieu de terrain polyvalent (peut jouer à tous les postes du milieu)
Ailier droit/gauche (attaquant, joue uniquement à droite/gauche)
Attaquant de pointe (avant-centre, taille > 1,9m , joueur physique)
Attaquant de pivot (avant-centre, joueur technique)
Attaquant polyvalent (peut jouer à tous les postes de l’attaque)

