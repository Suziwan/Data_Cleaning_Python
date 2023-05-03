# Data_Cleaning_Python
Week 2 Day 2 - Projects : Cleaning data for energy bills and air quality

## Project 1 : Energy Bills

L'objectif est de transformer le fichier récupéré en un fichier exploitable. Cela signifie qu'ils n'ont qu'à rechercher le nom d'une antenne en particulier, et ils peuvent obtenir l'historique de sa consommation d'énergie pour vérifier s'il y a des anomalies. Pour que cet historique soit intéressant, ils ont besoin d'avoir la consommation moyenne journalière (comme ça par exemple, ils peuvent comparer un mois de Février qui fait 28 jours avec un mois de janvier qui fait 31 jours, sans se dire que la diminution vient de la différence de jours dans un mois).  
Source: https://drive.google.com/file/d/1Xpfmecb4PmW-CEqFuiLdelZx4jWxZTD-/view?usp=sharing  

1) Le nom d'une antenne a un format bien précis : il est toujours composé de 4 chiffres et de deux lettres. On te demande de retirer tout autre caractère de la colonne "SITE_NAME".
2) On te demande de supprimer la colonne "INVOICE_NAME" qui n'apporte rien aux équipes.
3) Il y a des antennes pour lesquelles on a des factures mensuelles tandis que pour d'autres, on les reçoit moins régulièrement (trimestre, semestre, année). Ajoute une colonne à ton tableau qui calcule le nombre de jours entre le début de la période de facturation et la fin de la période de facturation.
4) A partir de cette nouvelle colonne, crée une autre colonne qui nous donne la consommation journalière moyenne de la période.
5) Merci d'ajouter également une colonne qui donne, pour chaque antenne, le nombre de factures dont on dispose au total. Pas grave si l'information se répète à chaque ligne pour une même antenne.
6) Et information bonus si tu y arrives : les équipes aimeraient beaucoup avoir une liste de toutes les antennes avec, pour chaque antenne, le coefficient de variation de la consommation. Cela permettra d'avoir une idée, pour chaque antenne, de la dispersion de sa consommation d'énergie.
7) Enfin, tu dois exporter ces deux fichiers obtenus pour pouvoir l'envoyer aux équipes de l'opérateur et leur demander si c'est bien cela qu'ils attendaient de toi.

## Project 2 : Air Quality

OpenAQ souhaiterait mettre en ligne sur son site un fichier qui permet de comparer des mesures de l'air récentes, relevées sur un jour donné, partout dans le monde. Pour cela, on te demande de nettoyer les données dont on dispose pour l'instant.  
Source: https://drive.google.com/file/d/1NnwIVdBng0Ct9rw-WfSEM6fGB9TtYcyv/view?usp=sharing

1) Supprimer les données qui ne concernent pas la journée du 06-08-2021.
2) Supprimer les données qui sont illisibles et pour lesquelles on ne comprend pas la ville concernée.
3) Pour chaque polluant, vérifier qu'on n'a qu'une seule mesure utilisée. Autrement, supprimer les données qui correspondent à la mesure minoritaire ou moins cohérente.
4) Regarder s'il y a des valeurs aberrantes ou des problèmes par rapport à notre objectif final (pouvoir comparer des mesures sur un maximum de pays) et noter ces aspects dans un fichier texte.
