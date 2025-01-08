# Réponses aux question : Introduction

**1. Le fichier est-il exploitable dans l'état ? Si nécessaire, comment doit-il être modifié ?**
     
   **Non**, le fichier n'est pas exploitable en l'état à cause la première ligne du fichier. La première ligne d'un jeu de donnée doit correspondre aux intitulés des variables en commençant par la première cellule de la première ligne et colonne (cellule A1 dans un tableur).  
     *NB : un jeu de données peut ne pas avoir d'en-tête avec les nom de variable et avoir directement des données dès la première ligne, le nom des variables est alors souvent consigner dans un document annexe.*  
  
**2. Que représente chaque ligne ?**
     
   Chaque ligne représente un **passage dans une salle de bloc opératoire**. Une 'ligne' dans un jeu de données est appelé ***une unité d'observation (ou unité statistique)***. Le choix de cette dernière selon la question posée / l'objectif est capitale.
   Dans notre cas, l'unité d'observation pourrait être un patient ou un séjour à l'hôpital : cela impliquerait d'agréger les données, en prenant par exemple, son premier passage (la notion d'agrégation sera abordée dans un autre chapitre) mais cela eneleverait une source dépendance entre les unités d'observation.
    
**3. Quelle colonne ou combinaison de colonne est une clé primaire (identifiant unique de chaque ligne) ?**  
  
   Dans ce jeu de données, aucune variable n'est individuellement une clé primaire : ici, plusieurs unité d'observation peuvent avoir la même date d'opération, le même IEP/IPP (reprise chirurgicale). Dans ce cas, 2 possibilités sont présentes :
   - il est possible de définir une clé primaire dite ***composite*** : la clé primaire est composée d'une combinaison de variables, on cherche alors à avoir une combinaison dite minimale : avec le moins de variable possible. Dans notre cas, une clé primaire composite pourrait être 'IPP' (ou 'IEP') + 'Date d'opération' + 'Patient en salle'. La combinaison 'IPP+Date d'opération' n'est pas suffisante car une reprise chirurgicale peut avoir lieu le même jour, la combinaison 'IPP+Patient en salle' non plus car un patient peut, théoriquement, être opéré à la même heure 2 jours différents.
   - le cas le plus fréquent est de créer une colonne remplissant ce rôle (on la nomme généralement 'id' ou 'index') : chaque ligne du jeu de donnée à alors 
6. Quelle est le type de variables attendu de chaque colonne ?
7. Quelle est le type de variables réelle de chaque colonne ?
8. Le jeu de données présente-t-il des variables non structurées ?
9. Au vu de la demande formulée, quelle colonne représente la variable à expliquer ?
10. Certaines variables vous semblent-t-elles dispensables pour l'analyse ?
