[Aanmaken van een Workspace Collection in Microsoft Azure]:/create-workspace-collection.md
[Rapport maken en toevoegen aan de workspace]:/create-add-report.md
[Rapport integreren in een webpagina]: /integrate-report.md
[Wat is Microsoft Power BI Embedded]: /README.md

# Aan de slag met Microsoft Power BI Embedded

Microsoft komt nu met Power BI als onderdeel van de office 365 Suite. Microsoft Power BI Embedded biedt de mogelijkheid om geavanceerde rapportages eenvoudig te integreren in een maatwerkapplicatie. In deze snelstart willen we door middel van een aantal stapen laten zien hoe wij Power BI integreren in onze maatwerkapplicaties.

* [Wat is Microsoft Power BI Embedded]
* Aanmaken van een Workspace Collection in Microsoft Azure
* [Rapport maken en toevoegen aan de workspace]
* [Rapport integreren in een webpagina]

In vervolg op [Wat is Microsoft Power BI Embedded] gaan we nu een Workspace Collection creeren.

## Aanmaken van een Workspace Collection
Voordat we kunnen beginnen met het toevoegen van rapporten hebben we eerste een Workspace Collection nodig. Voor het aanmaken van een Workspace Collection moet je in het bezit zijn van een Microsoft Azure Subscription. 

1. Open de Azure Portal: https://portal.azure.com 

2. Klik **+ New** boven in het menu

    ![Stap2](/content/ife-create-workspace-collection-step-2.png "Stap2")

3. Onder **Data + Analytics** klik Power BI Embedded
4. Op de **Workspace Collection Blade** moeten verplichte velden worden ingevoerd

    ![Stap 4](/content/ife-create-workspace-collection-step-4.png "Stap 4")

5. Klik **Create**

De Workspace Collection wordt nu aangemaakt. Wanneer deze compleet is wordt er een notificatie gegeven ‘Deployments succeeded’ wordt de klik op de notificatie en de Workspace Collection Blade getoond.

![Blade](/content/ife-create-workspace-collection-blade.png "Blade")

## Power BI Api Keys
Om gebruik te maken van de Workspace Collection zijn de Api Keys nodig. Deze api-keys zorgen ervoor dat een applicatie kan communiceren met de workspace collection.

De api-keys kunnen we vinden aan de linkerkant van op de Workspace Collection Blade.

![Blade](/content/ife-create-workspace-collection-accesskeys.png "Blade")

Nu we een workspace collection tot onze beschikking hebben met daarbij de behorende access key kunnen we een [Rapport maken en toevoegen aan de workspace].