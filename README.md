# Énoncé 243-421-H24 TP1 - Réception d'une trame NMEA

## Matériel 

- 1 Carte PIC 
- 1 PIC KIT 4 
- 1 Écran LCD série 
- 1 câble USB 
- 1 Analyseur Logic16 

## Manipulations

1. Créer un nouveau projet et le configurer à l’aide de MCC.  
   Consulter https://youtu.be/TPaN5uCsp0I au besoin. 
2. Faire le logigramme d’une machine d’état qui se synchronise sur les 6 premiers caractères d’une trame RMC du protocole NMEA ($GPRMC,). 

3. Écrire un programme qui : 
    - Reçoit sur son UART (EUSART1). 
    - Utilise une machine d’état (incluant obligatoirement enum, switch case et typedef) pour se synchroniser sur la trame RMC du protocole NMEA.
    - Change l’état de la DEL (A5) sur réception d’une trame valide ($GPRMC,). 
 
4. Utiliser l’application TeraTerm pour transmettre des trames NMEA d’un fichier texte vers l’interface UART du PIC. 

1. Utiliser le PICKit 4 pour programmer et debugger la carte PIC. 

1. Utiliser l’analyseur Logic 16 pour visualiser les trames NMEA reçues. 
 
# Évaluation 

1. Remettre tous les fichiers du projet. 
  - Le programme doit être bien commenté et contenir un entête complet.
  - Tous les fichiers requis pour recompiler le projet sont nécessaire 
 
2. Faire valider le fonctionnement, l’utilisation du debugger et l’utilisation de l’analyseur Logic16. 

# Extra 

  Cette section est optionnelle, elle donne jusqu’à 10% de bonus. 
  
  L’extra consiste à configurer le uart en interruption, à récupérer l’heure de la trame RMC (les 6 caractères suivants la virgule) puis de l’afficher sur le LCD que vous aurez connecté sur la carte PIC (EUSART1). 
