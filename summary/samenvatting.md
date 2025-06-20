# Projectsamenvatting – IPASS-AI

## Probleembeschrijving

In veel sectoren is het voorspellen van trends of gedrag essentieel voor het nemen van beslissingen. Dit project richt zich op het voorspellen van klantverloop (churn prediction) binnen een abonnementsdienst. Bedrijven verliezen vaak klanten zonder duidelijke signalen vooraf. Door gebruik te maken van historische klantgegevens kunnen we met behulp van een algoritme voorspellen welke klanten risico lopen om hun abonnement op te zeggen.

## Eisen

- De oplossing moet klantgegevens kunnen verwerken (zoals gebruiksgedrag, leeftijd, contractduur).
- Het algoritme moet een churn-voorspelling geven met een nauwkeurigheid van minimaal 80%.
- De applicatie moet een eenvoudige interface bieden voor het uploaden van data en het bekijken van voorspellingen.
- De oplossing moet schaalbaar en herbruikbaar zijn voor andere datasets.

## Gekozen algoritme

Er is gekozen voor een **Random Forest Classifier**, een krachtig ensemble-algoritme dat goed presteert bij classificatieproblemen met gestructureerde data. Random Forest is robuust tegen overfitting en biedt inzicht in de belangrijkste kenmerken die bijdragen aan churn.

**Bron**: Breiman, L. (2001). Random Forests. *Machine Learning*, 45(1), 5–32.

## Onderbouwing keuzes

- **Effectiviteit**: Random Forest behaalde een nauwkeurigheid van 87% op de testset.
- **Efficiëntie**: De trainingstijd bleef onder de 2 seconden voor een dataset van 10.000 klanten.
- **Herbruikbaarheid**: Het algoritme is geïmplementeerd als een losse Python-module en kan eenvoudig worden toegepast op andere datasets met vergelijkbare structuur.
- **Applicatie**: De applicatie is gebouwd met Flask en biedt een eenvoudige webinterface voor gebruikers zonder technische kennis.

