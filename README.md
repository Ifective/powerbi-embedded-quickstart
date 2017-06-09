[Aanmaken van een Workspace Collection in Microsoft Azure]:/create-workspace-collection.md
[Rapport maken en toevoegen aan de workspace]:/create-add-report.md
[Rapport integreren in een webpagina]: /integrate-report.md
[Wat is Microsoft Power BI Embedded]: /readme.md

# Aan de slag met Microsoft Power BI Embedded

Vandaag de dag wordt de vraag naar rapportages in  maatwerkapplicaties steeds groter. Applicaties slaan steeds meer informatie op. De opgeslagen informatie willen we inzichtelijk maken met geavanceerde rapportages. Deze rapportages lijken vaak simpel, maar waar nodig dient de complexiteit van data zichtbaar te zijn en er moet eenvoudig 'ingezoomd' kunnen worden op data. 

Microsoft komt nu met Power BI als onderdeel van de office 365 Suite. Microsoft Power BI Embedded biedt de mogelijkheid om geavanceerde rapportages eenvoudig te integreren in een maatwerkapplicatie. In deze snelstart willen we door middel van een aantal stapen laten zien hoe wij Power BI integreren in onze maatwerkapplicaties.

* Wat is Microsoft Power BI Embedded
* [Aanmaken van een Workspace Collection in Microsoft Azure]
* [Rapport maken en toevoegen aan de workspace]
* [Rapport integreren in een webpagina]

## Microsoft Power BI
Microsoft Power BI is een analytische tool om data te analyseren uit een of meerdere databronnen om vervolgens deze data te delen met eindgebruikers. Met behulp van 'fancy' rapporten en dashboards kan data eenvoudig gepresenteerd en gedeeld worden op diverse apparaten. 

Microsoft Power BI biedt mogelijkheden om aansluiten op verschillende databronnen. Hierbij kunnen we denken aan Excel, platte tekstbestanden of SQL Server in de cloud of on-premise.

Met behulp van Power Bi Desktop kan men de data uit verschillende databronnen laten samenkomen in datasets. Op deze samengestelde datasets kunnen diverse rapportages en dashboards worden gemaakt. Power Bi Desktop is een gratis desktopapplicatie wat lokaal op een computer geïnstalleerd kan worden. De rapportages gemaakt met Power Bi Desktop worden vervolgens via de Power Bi Service getoond aan eindgebruikers. 

Microsoft Power BI is onderdeel van Office 365. De basis mogelijkheden zijn gratis te gebruiken. Bij wat geavanceerde functionaliteiten dienen licenties gekocht te worden via Office 365. Na toewijzing van een licentie kan een gebruiker direct aan de slag.

Meer informatie over powerbi is te vinden op [powerbi.microsoft.com](https://powerbi.microsoft.com/en-us/what-is-power-bi/  "https://powerbi.microsoft.com/en-us/what-is-power-bi/").

![Overview](/content/ife-power-bi-overview.png "Overzicht van Power BI")

## Microsoft Power BI Embedded
Microsoft Power BI Embedded is een Azure dienst. Deze dienst maakt het mogelijk om een rapport gemaakt in Power BI desktop, te integreren in webapplicaties of mobiele apps. Het biedt een applicatieontwikkelaar de mogelijkheid om in een maatwerkapplicatie, met zijn eigen set aan requirements, complexe rapporten te integreren via de Power Bi Service.

Het gebruik van Power BI Embedded zorgt ervoor dat een Power BI (Office365) account niet nodig is. De dienst staat los van Office 365, het is een dienst in Microsoft Azure. In plaats van betalen van licentiekosten wordt er betaald op basis van een ‘sessies’. Als een rapport wordt geopend in de applicatie door een eindgebruiker dan wordt er voor deze eindgebruiker een sessie aangemaakt. 

## Microsoft Power PI Embedded overzicht
Microsoft BI Embedded bestaat uit een aantal onderdelen. in de onderstaande afbeelding worden de onderlinge relaties tussen de onderdelen weergegeven. 

![Overview Embedded](/content/ife-power-bi-embedded-overview.png "Overzicht van Power BI Embedded")

* **Microsoft Azure Subscription**: Voor het gebruik van Power BI Embedded is een Microsoft Azure Subcription noodzakelijk. In een subscription kunnen meerdere Workspace Collections worden aangemaakt.

* **Workspace Collection**: Een Workspace Collection is een verzameling van 0 of meerdere Workspaces. Een workspace Collection wordt gemaakt in een bepaalde region (bv. West-Europe). In een Workspace Collection bevinden zich de accesskeys en defenities van gebruikers en rollen. 

* **Workspace**: Een Workspace is een container voor de daadwerkelijke content, dit betreft de rapporten en de datasets. 

Door de gekozen structuur bij Power BI embedded kan bij het inrichten van een Power BI omgeving meerdere keuzes worden gemaakt. Wanneer maak ik een Workspace Collection, wanneer een Workspace etc. Keuze zijn afhankelijk van de requirements, bijvoorbeeld beveiliging of ondersteuning van meerdere Azure Regions. 
Voor Ifective wordt in de meeste gevallen een Workspace Collection per omgeving aangemaakt (klant/OTAP) en binnen de Workspace Collection per afdeling een workspace.

Volgende stap: [Aanmaken van een Workspace Collection in Microsoft Azure] 