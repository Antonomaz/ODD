# ODD - Antonomaz

Ce répertoire contient les schémas de validation XML des fichiers encodés ainsi que la documentation de l'ensemble de l'encodage. 

/!\ L'ODD n'est plus à jour depuis juin 2023: se fier au schéma RNG. 

## Schéma de validation

Le schéma RNG produit à partir de l'ODD est utilisé pour s'assurer de la conformité de l'encodage de chaque fichier du corpus aux règles d'encodage préalablement définies.
Il se trouve dans le dossier [Schéma](https://github.com/Antonomaz/ODD/blob/master/Schema).

Pour s'assurer de ladite conformité de chaque fichier XML encodé, il convient d'y lier le schéma RNG produit :
* soit en téléchargeant le schéma localement, on ajoutera alors ces deux lignes en tête de chaque fichier :
```xml
<?xml-model href="/chemin/vers/ODD_Antonomaz.rng"
            type="application/xml"
            schematypens="http://purl.oclc.org/dsdl/schematron"?>
<?xml-model href="/chemin/vers/ODD_Antonomaz.rng"
            type="application/xml"
            schematypens="http://purl.oclc.org/dsdl/schematron"?>
``` 
* soit en faisant directement référence au schéma accessible en ligne (une connexion internet est alors nécessaire pour valider le fichier), en précisant :
```xml
<?xml-model href="https://raw.githubusercontent.com/Antonomaz/ODD/master/Schema/ODD_Antonomaz.rng"
            type="application/xml"
            schematypens="http://relaxng.org/ns/structure/1.0"?>
<?xml-model href="https://raw.githubusercontent.com/Antonomaz/ODD/master/Schema/ODD_Antonomaz.rng"
            type="application/xml"
            schematypens="http://purl.oclc.org/dsdl/schematron"?>
```

## Documentation de l'encodage

Le dossier [Documentation](https://github.com/Antonomaz/ODD/blob/master/Documentation) contient la documentation de l'encodage au format HTML.

Vous y trouverez notamment des précisions au sujet des choix d'encodage du projet Antonomaz.


**L'ODD, en cours de finalisation, est susceptible d'évoluer.**
