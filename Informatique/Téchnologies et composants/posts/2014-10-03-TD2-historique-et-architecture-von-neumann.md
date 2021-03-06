title: TD2, Historique et architecture Von Neumann 

<small>Cours par **M.BLOYET**, [contact].</small>

## Historique

### Antiquité

-3000 av. Jesus-Christ : Le pentagramme de Fuhi. 




    ▒ ▒   ▒ ▒  ▒ ▒   ▒ ▒  ▒▒▒  ▒▒▒  ▒▒▒  ▒▒▒
    ▒ ▒   ▒ ▒  ▒▒▒   ▒▒▒  ▒ ▒  ▒ ▒  ▒▒▒  ▒▒▒
    ▒ ▒   ▒▒▒  ▒ ▒   ▒▒▒  ▒ ▒  ▒▒▒  ▒ ▒  ▒▒▒
    ^-0   ^-1  ^-2   ^-3  ^-4  ^-5  ^-6  ^-7

C'est une sorte de «code barre» qui représente les inscriptions binaires. 
Une barre pour un 1. Deux carrés pour un 0. Suite à cela, un grand vide. 

### Moyen âge

Ensuite, au moyen âge, le système comptable étant devenu indispensable pour 
le prélèvement de l'impôt, on utilise des calculateurs à roue. 

C'est Pascal, en s'inspirant du boulier chinois (-700 av. JC), qui crée la 
"Pascaline". C'est une machine à roues crantées. 

### Monde industrialisé

Charles Babbage améliore ensuite la Pascaline (en 1812), qui permet de 
faire des opérations sur des nombres beaucoup plus grands, et des 
nombres à virgule flottante. 

### XXème siècle

En reprenant tout les travaux précédents, VonNeumann, un hongrois chercha, 
pendant la seconde guerre mondiale a créer une machine dite «Électronique». 
VonNeumann fût à l'époque un exilé aux États-Unis, né en 1903 et mort en 
1957. 

Il participait déjà aux projets sur la mécanique quantique, aux projets sur 
la bombe atomique, à l'informatique (machine VonNeumann, 1945) et à 
l'automatisme cellulaire. 

Les recherches de VonNeumann ont permis la création de LENIAC. C'est la 
première machine de calcul électronique réalisée à partir de l'architecture 
VonNeumann. Cette machine utilise des tubes à vide. (17 468 tubes). 
Pour mémoriser les programmes de sa machine, on utilise des cartes perforées. 

Ensuite, émerge un modèle avec mémoire magnétique. C'est le premier 
disque dur. Créé par International Business Machine (IBM) en 1956. 
5 millions de caractères. C'est inférieur à 5Mo. 

En 1982, arrivée du premier PC. Par IBM. L'IBMPC. 

En 1976, l'Apple Computer, machine avec boite en bois. 

## Introduction à la technologie des ordinateurs. 

### Introduction

Nous utilisons tous des ordinateurs, qui est la traduction du terme 
«computer» en anglais. 

**Ordinateur** : Système de traitement automatisé de l'information qui 
reçoit des données en entrée, effectue un traitement logique afin de les 
afficher sous forme de  résultat en sortie. 

En france, un certain Perret, a choisi "Ordinateur" pour désigner «PC», 
pour l'académie Français. Du latin *ordinare*. Machine qui met de l'ordre 
dans les données. 

### L'approche en blocs fonctionnels

Un ordinateur est décomposé en bloc spécialisés qu'on appel 
«Blocs fonctionnels». 

Notamment, trois blocs essentiels, C'est l'approche retenue par 
VonNeumann :

* Entrées : *Input*
* Sorties : *Output*
* Traitement : *Processing*, lui même décomposé en trois parties. 
    * Commandes
    * Instructions données (jeu d'instruction)
    * Unité de calcul ou "Co-processeur Arithmétique"
    * Une Mémoire vive, 
        qui sert à récupérer et utiliser les données relatives au traitement. 

&nbsp;

    | Entrées | --> | Système de traitement | --> | Sorties |
    |         |     |                       |     |         |
    |         |     |  Commandes, mémoires, |     |         |
    |         |     |    Unité de calcul    |     |         |


La **mémoire vive** est **volatile**, car il est nécessaire de l'alimenter en 
permanence pour maintenir son contenu. Celà est du au fait que cette mémoire 
est faite de transisors. 

Est associée à celle-ci une **mémoire morte**, qui va stocker 
l'information de manière «indélébile» de manière à ce qu'elle soit 
disponible après un redémarrage. Cette mémoire stock notamment des 
informations de configuration périphériques. 

Elle est en relation avec des mémoires dites **auxiliaires ou externes**. 
Celles ci permettent de stocker des fichiers. 

Toutes ces mémoires périphériques ou externes sont reliées à l'unité de 
calcul par un bus. Il y a une multitude bus, nommés selon la type de 
périphérique (USB, IDE, ATA, SATA, etc.)

Pour gérer l'utilisation d'un bus, il faut un contrôleur, dont le rôle est 
de mettre en relation certains périphériques et de s'assurer de la bonne 
transmission de l'information. Ces contrôleurs portent le même nom que la 
technologie du périphériques, (USB, IDE, ATA, SATA, PCIx, etc.).
Ces contrôleurs sont des puces électroniques. 

Il en existe 2 :

* North bridge : (Échanges rapides) Mémoire centrale, carte vidéo
* South bridge : (Échanges lents)   Mémoires type disque dur, 
    périphériques USB, carte réseau. 

C'est ce type d'architecture qui a été utilisé par VonNeumann et qui est 
toujours utilisé actuellement. 

### L'unité Centrale de Traitement de l'Information

En anglais, *Central Processing Unit*, Unité Centrale de Traitement. 

#### L'unité Centrale

Il ne s'agit pas du boîtier d'ordinateur. 

L'unité Centrale comprend les elements suivants:

* L'Unité Centrale de Traitement. 
* La mémoire centrale. 
* Les bus qui les relient. 

#### L'Unité centrale de Traitement. 

**L'unité de commande** est le premier élément de l'UCT. Elle gère le bon 
fonctionnement des opérations de traitement. C'est à dire le bon 
déroulement d'un programme. Elle synchronise donc toutes les opérations à 
effectuer. Elle possède donc sa propre mémoire stockant l'ensemble des 
opérations devant être effectuées, (Registre). 

Une **Unité de calcul**, appelée également coprocesseur Arithmétique, (UAL) 
*Arithmetical & Logical Unit (ALU)* a pour rôle de convertir et de traiter 
l'ensemble des données numériques. 

La **mémoire centrale** ou RAM *Random Access Memory* est une 
«mémoire à accès aléatoire», car elle est accéssible à une adresse 
différente sans (gros) délai, comme il peut y en avoir avec un support 
mécanique (disque dur). Les cellules sont accessibles par une adresse 
mémoire, représentée en hexadécimale, de taille différente selon la taille du 
**mot mémoire**. 

L'unité d'échange: Elle gère ce qui n'est pas interne à l'unité 
centrale de traitement. C'est à dire les périphériques. 

##### Les périphériques 


    Carte Mère
    
    [ UCT ]
       |
       |
       v
    [ North Bridge ] -------------> [ Carte video, etc. ]
       |
       |
       v
    [ South Bridge ] -------------> [ Périphériques ]

* Périphériques d'entrée
    * Clavier
    * Souris
    * Écran tactile
    * stylet
    * tablette graphique
    * lecteur de code barre
    * Périphériques d'image
        * Webcam
        * Scanner
    * Périphériques de communication
        * Carte réseau
        * Carte wifi
        * Carte modem
        * Carte d'acquisition
    * Périphériques de stockage
        * USB
        * Lecteur CD/DVD ROM
    * Périphériques de son
        * Microphone
        * Acquisition
* Périphériques de sortie
    * Casque, enceintes
    * Imprimante
    * Écran
    * 
* Périphériques de communication
    * Carte réseau
    * Carte wifi
    * Carte modem
    * Carte d'acquisition

#### Étude de l'UCT

L'UCT gère les données par l'intermédiaire de programmes informatiques. 

Un programme est une suite d'opérations à effectuer produisant un 
résultat. L'ensemble de ces opérations s'appelle des instructions. C'est à 
dire une opération élémentaire comprise par un processeur. 

Ces instructions sont gérées par l'unité de commandes. 

Les instructions sont composées de deux parties. «Ce qu'il faut faire» 
(L'instruction, dans la zone d'opération), 
et «avec quoi le faire» (l'adresse des données, dans la zone adresse). 

La partie opération est gérée par un langage **Évolué**, **de haut niveau**. 
Ce langage est traduit par les machines en langage de bas niveau. C'est le 
langage assembleur. 

Ces instructions correspondent à des micro-commandes exécutées par l'UCT. 
Elles sont gravées à l'avance par les fondeurs informatiques. 
Cela représente un jeu d'instruction. 

Par exemple:

    CMP <Adresse_cible_donnée> <Adresse_cible_donnée> ; CMP  
    JNE <Adresse_cible_instruction> ; Veut dire «Jump If not Equal» et 
    ; apparait à partir de l'architecture x86

La **zone opération** est divisée en deux parties: le code de 
l'opération, décodable par la machine et suivi d'un code complémentaire, 
correspondant à la nature de l'opération à effectue. 

La **zone adresse** contient elle la valeur hexadécimale de la céllule à 
utiliser pour l'opération. 

Il existe différentes manières de joindre l'information. C'est l'adressage. 

* Par une valeur       : «Va en D4»
* Par une localisation : «Va dans le registre D»
* Une «transaction»    : «Va en D4 + 2»

Exemple en assembleur:

    jmp $0x3e4f      ; Va à l'adresse 0x3e4f
    jmp %eax         ; Va à l'adresse indiquée par le registre EAX
    jmp $0x00b4+%eax ; Va à l'adresse $0x00B4h + le contenu du registre EAX

Ces adresses sont utilisées par l'UAL. 

### Les composants réels de l'UCT

<!-- TODO: intégrer le schémas 7.5 -->

~~~text
| RAM         |
|-------------|             ^ ^ ^ ^ ^ ^ ^ ^ ^
|             |             | | | | | | | | |
|             |            |``````````````````|
|             |            |  Microcommandes  |
|             |            |__________________|
|             |               ^                
|             |               |                
|             |               |                
| …           |  |````|    |````````````|     |`````````````````|
| Instr. 6    |  | CO |<-- | Séquenceur | --> | Registre d'état |
| Instr. 5    |  |____|    |____________|     |_________________|
| Instr. 4    |               ^        
| Instr. 3    |               |        
| Instr. 2    |            |``````````|
| Instr. 1    | ---------> | Décodeur |
                           |__________|
~~~

CO = Compteur Ordinal

RI = Registre d'Instruction

Un programme est exécute depuis le disque dur. 
Il est alors chargé dans la mémoire centrale sous la forme de série(s) 
d'instructions. Le compteur ordinal pointe sur la première instruction 
exécutée. Au deuxième cycle d'Horloge (CH), cette instruction est chargée 
dans le décodeur, pour la partie **zone opération**. 

Le décodeur transforme l'instruction évoluée en une micro-commande 
utilisable par du materiel. 

Le code simplifié est envoyé au séquenceur. Son rôle est de générer 
les micro-commandes a destination des périphériques concernés au rythme 
de l'horloge. 

Le séquenceur envoie au registre d'état des données sur le bon déroulement 
de l'opération. Réussite ou échec, avec un code pour l'instruction et un 
*flag* (drapeau). 

Dés qu'une microcommande est générée, le compteur ordinal incrémente 
l'adresse de l'instruction à exécuter. (L'adresse de l'instruction est un 
pointeur sur l'instruction à exécuter.) 

#### Le fonctionnement de l'UCT

Les micro-commandes générées par le séquenceur sont envoyées directement à 
l'UAL, composant électroniques composé d'additionneurs, soustracteurs, 
multiplicateurs, diviseurs, logiques (ET,OU,NON). 

Cette UAL est composée d'un accumulateur et de registres de calcul 
temporaires. On parle également de coprocesseurs arithmétiques. Son rôle 
va être de traduire les adresses (représentées en hexadécimales) des 
données en valeurs utilisables pour le traitement. 

**<span style="color:red;"> v--- BEGIN RÉSUMÉ! ---v </span>**

L'UAL, couplée à L'UCT, va donc 

1. Acquerir et décoder les Instructions. 
2. Executer les calculs (ou opérations). 
3. Gérer les adresses des Instructions. 
4. Mémoriser l'état interne de traitement. (Réussite/Échec)
5. Générer les signaux de commande. 

**<span style="color:red;"> ^--- END RÉSUMÉ! ---^ </span>**

### Les differents types de bus. 

On parle de bus système lorsqu'il relie la mémoire centrale au processeur. 
Le bus système est composé de 3 bus distincts. À chaque type de données 
son bus. 

* Le bus de commande
* Le bus d'adresse
* Le bus global

#### Le bus de donnée

*Data Bus*

Son rôle est de véhiculer les instructions. Il a une certaine 
largeur. La largeur correspond à la taille maximale qu'il peut transporter. 
Un fil par bit. Les données peuvent aller de la mémoire à l'UCT ou de l'UCT 
à la mémoire. 

#### Le bus d'adresse

*Address Bus*

Il ne véhicule que la zone adresse d'une instruction. 

Il peut la stocker dans un registre particulier: le registre d'adresse 
d'un coté et 
dans l'accumulateur. 

Le bus d'adresse va permettre de déterminer la taille de mémoire 
utilisable. Les adresses sont unidirectionnelles. 

#### Le bus de commande

Il sert a véhiculer les codes opération. 

[contact]:mailto: "Email du professeur"
