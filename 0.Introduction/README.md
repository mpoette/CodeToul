# Préambule

## Objectif de ce chapitre

- Mettre en forme un jeu de données
- Faire une première inspection d'un jeu de données
- Comprendre les limites d'Excel concernant la manipulation de datasets

## Mise en situation

Vous êtes contacté pour traiter et analyser un jeu de données afin de répondre à la question suivante :
*« Le type d'anesthésie réalisée est-il corrélé à la durée d'occupation de la salle d'opération »*.

Le jeu de données contient les colonnes suivantes :

- **Date opération :** date de la chirurgie
- **IEP :** identifiant du séjour
- **IPP :** identifiant du patient
- **Age :** âge du patient
- **Classe ASA :** score ASA du patient compris entre 1 (patient sans comorbidité) et 5 (patient moribond). Peut être suivie de la lettre U si l'intervention est prévue moins de 48 heures après l'évaluation anesthésique.
- **Intervention princ :** intitulé de l'intervention
- **Bloc :** unité de bloc opératoire
- **Type anesthésie :** type d'anesthésie réalisée
- **Type d'hospit :** mode d'hospitalisation du patient
- **Priorité médicale :** chirurgie programmée ou non programmée
- **Type anesthésie :** type d'anesthésie réalisée
- **Arrivée SAS d'accueil :** heure d'arrivée au SAS d'accueil
- **Arrivée SAS ALR :** Heure d'arrivée au SAS ALR
- **Patient en salle :** un arrivée du patient en salle d'opération
- **Début d'anesthésie :** heure du début du temps anesthésique
- **Anesthésie prête :** heures de fin du temps d'induction de l'anesthésie
- **Début intervention :** début de l'intervention chirurgicale
- **Fin intervention :** heure de fin de l'intervention chirurgicale
- **Fin anesthésie :** heures de fin de l'anesthésie
- **Sortie de salle :** heure de sortie du patient de la salle d'opération
- **Arrivée SSPI :** Heure d'arrivée en salle de surveillance post interventionnelle
- **Sortie autorisée SSPI :** heure à partir de laquelle le patient est autorisé à sortir de SSPI
- **Sortie SSPI :** départ du patient de la SSPI

## Préambule : analyse de la structure du jeu de données**

1. Le fichier est-il exploitable dans l'état ? Si nécessaire, comment doit-il être modifié ?
2. Que représente chaque ligne ?
3. Quelle colonne ou combinaison de colonne est une clé primaire (identifiant unique de chaque ligne) ?
4. Quelle est le type de variables attendu de chaque colonne ?
5. Quelle est le type de variables réelle de chaque colonne ?
6. Le jeu de données présente-t-il des variables non structurées ?
7. Au vu de la demande formulée, quelle colonne représente la variable à expliquer ?
8. Certaines variables vous semblent-t-elles dispensables pour l'analyse ?
    6.2 Cellule de code vs markdown
    6.3 ouvrir un fichier Excel
    6.4 Inspection d'un dataframe (type, forme)
    
