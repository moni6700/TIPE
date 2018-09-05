# TIPE 2016 - �tude et mod�lisation d�un syst�me proie-pr�dateur

## Sommaire
* [A propos de ce TIPE](#a-propos-de-ce-tipe)
    * [Installation](#installation)
    * [Screenshots](#screenshots)
* [Introduction](#introduction)
* [Plan d'�tude](#plan-d�tude)
* [Conclusion](#conclusion)
* [Bibliographie](#bibliographie)

## A propos de ce TIPE
J'ai pr�sent� mon [TIPE](https://fr.wikipedia.org/wiki/Travail_d%27initiative_personnelle_encadr%C3%A9) en juin 2016 (avant la r�forme de 2017). C'�tait l'un de mes premiers gros projet en Python. Pour la grille principale, j'ai repris une partie du code d'un Jeu de la Vie r�alis� l'ann�e d'avant. Avec du recul, le script Python est tr�s mal �crit: surcomment�, une m�ga-classe englobant tout le programme, pas du tout optimis� et m�me tr�s lent sur certaines machines... mais il fonctionne toujours et les r�sultats restent int�r�ssants. C'est ce qui m'a pouss� � cr�er ce d�p�t public qui regroupe le programme de simulation, mon rapport et sa source LaTeX et les transparents de pr�sentation. Vous trouverez dessous les pr�-requis d'installation ainsi que le contenu de ma fiche synoptique de l'�poque qui pr�sente mon projet.

### Installation
Le programme de simulation se trouve dans `Programme/simulation.py` et n�cessite **Python 3+** avec les modules `tkinter`, `numpy`, `pickle` et `matplotlib` install�s. Le script est encod� en **UTF-8**.

### Screenshots

![Start](Screenshots/start.png)

![Running](Screenshots/running.png)

![Graphe](Screenshots/graphe.png)

## Introduction
La dynamique des populations est une branche des math�matiques et de l��cologie qui s�int�resse aux variations de la population d�une esp�ce, en tenant compte de l�influence du milieu et des interactions inter-esp�ces. De nos jours, avec la prise de conscience collective de la fragilit� des �cosyst�mes, ce domaine des sciences est devenu essentiel dans la lutte pour la pr�servation de la faune et de la flore.

Mon �tude se limite ici � un �cosyst�me constitu� de deux esp�ces, l�une faisant office de proie et l�autre de pr�dateur. De plus, l��volution des effectifs est suppos�e continue dans le temps et d�terministe, c�est-�-dire r�gie par des �quations diff�rentielles et par la donn�e d�un �tat initial. 

L�objet de mon expos� est de comprendre comment mod�liser th�oriquement les fluctuations des populations d�un couple proie-pr�dateur, avant d�en proposer une simulation informatique r�aliste � travers l�impl�mentation d�un automate cellulaire graphique sous Python.

## Plan d'�tude
J�aborde d�abord les �quations proie-pr�dateur de *Lotka-Volterra* et le comportement de ses solutions pour les confronter � une �volution r�elle de populations. Cette premi�re approche me permet ainsi de poser les fondements d�une adaptation informatique, aboutissant au d�veloppement d�un automate cellulaire param�trable et dynamique simulant le comportement des esp�ces dans leur habitat. C�est enfin avec ce programme que je me suis int�ress� � l�influence du milieu et des variables propres aux esp�ces sur la dynamique et la stabilit� des deux populations.

## Conclusion
Finalement, j�ai pu traduire un processus complexe sous forme d�interactions simples entre individus � l�aide de divers outils informatiques: automate cellulaire, programmation objet, interface graphique, analyse num�rique, manipulation de tableaux et de graphiques; ce qui m�a ensuite permis d�interpr�ter le r�le de chacun des param�tres en jeu.

## Bibliographie
* Alexander Dewdney, "Sharks and fish wage an ecological war on the toroidal planet Wa-Tor", Scientific American December, 1984.
* Jean-Ren� Chazottes & Marc Monticelli, "Sur les mod�les proie-pr�dateur en �cologie", http://www.espace-turing.fr/Sur-les-modeles-proie-predateur-en.html, 2013.
* Gr�gory Vial, Le syst�me proie-pr�dateur de Volterra-Lotka, 2011.
* G�rard Swinnen, Apprendre � programmer avec Python 3, Eyrolles, 2012.
