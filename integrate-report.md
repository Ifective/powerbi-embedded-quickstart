[Aanmaken van een Workspace Collection in Microsoft Azure]:/create-workspace-collection.md
[Rapport maken en toevoegen aan de workspace]:/create-add-report.md
[Rapport integreren in een webpagina]: /integrate-report.md
[Wat is Microsoft Power BI Embedded]: /readme.md
[Report Embed Sample]: https://microsoft.github.io/PowerBI-JavaScript/demo/code-demo/index.html

# Aan de slag met Microsoft Power BI Embedded

Microsoft komt nu met Power BI als onderdeel van de office 365 Suite. Microsoft Power BI Embedded biedt de mogelijkheid om geavanceerde rapportages eenvoudig te integreren in een maatwerkapplicatie. In deze snelstart willen we door middel van een aantal stapen laten zien hoe wij Power BI integreren in onze maatwerkapplicaties.

* [Wat is Microsoft Power BI Embedded]
* [Aanmaken van een Workspace Collection in Microsoft Azure]
* [Rapport maken en toevoegen aan de workspace]
* Rapport integreren in een webpagina

In vervolg op [Rapport maken en toevoegen aan de workspace] gaan we nu het rapport benaderen via een webpagina.

## Test integratie via Report Embed Sample
Voordat we het rapport gaan integreren in een maatwerk applicatie kunnen we met behulp van een aantal gegevens ons rapport testen in de [Report Embed Sample].

We hebben hiervoor de een report-id en een embed-token nodig. Deze gegevens hebben we in de vorige stap [Rapport maken en toevoegen aan de workspace] kunnen verzamelen.

![Power BI Desktop](/content/embed-sample.png "Power BI Desktop")

## Integratie in een webpagina
De voorbeelden zoals deze worden geschetst in [Report Embed Sample] kunnen wij ook toepassen in onze maatwerkapplicatie. Hiervoor dienen we de javascript library te installeren.

Install via Nuget:

    Install-Package Microsoft.PowerBI.JavaScript -Pre

Install from NPM:

    npm install --save powerbi-client

Install from Bower:

    bower install powerbi-client --save

    