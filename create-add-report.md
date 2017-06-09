[Aanmaken van een Workspace Collection in Microsoft Azure]:/create-workspace-collection.md
[Rapport maken en toevoegen aan de workspace]:/create-add-report.md
[Rapport integreren in een webpagina]: /integrate-report.md
[Wat is Microsoft Power BI Embedded]: /README.md

# Aan de slag met Microsoft Power BI Embedded

Microsoft komt nu met Power BI als onderdeel van de office 365 Suite. Microsoft Power BI Embedded biedt de mogelijkheid om geavanceerde rapportages eenvoudig te integreren in een maatwerkapplicatie. In deze snelstart willen we door middel van een aantal stapen laten zien hoe wij Power BI integreren in onze maatwerkapplicaties.

* [Wat is Microsoft Power BI Embedded]
* [Aanmaken van een Workspace Collection in Microsoft Azure]
* Rapport maken en toevoegen aan de workspace
* [Rapport integreren in een webpagina]

In vervolg op [Aanmaken van een Workspace Collection in Microsoft Azure] gaan we nu een Rapport maken en toevoegen aan een **Workspace**.

## Power Bi Rapport maken

Zoals al aangegeven kan er een rapport worden gemaakt in Power BI Desktop. Power BI Desktop kan worden gratis gedownload via [https://powerbi.microsoft.com/en-us/desktop/](https://powerbi.microsoft.com/en-us/desktop/)

![Power BI Desktop](/content/ife-power-bi-desktop.png "Power BI Desktop")

Het resultaat uit Power BI Desktop is een bestand met .pbix extentie. Dit bestand gaan we uiteindelijk toevoegen aan een **Workspace**.

Als je Power BI niet kan downloaden of je hebt geen inspiratie om een rapport te maken dan is het ook mogelijk om een [demo bestand](http://go.microsoft.com/fwlink/?LinkID=780547) te downloaden van de Microsoft. 

## Bestand toevoegen aan een Workspace Collection

Zoals we hebben kunnen lezen in [Wat is Microsoft Power BI Embedded] wordt een rapport toegevoegd aan een **Workspace**. Voordat we een rapport kunnen uploaden dienen ook een Workspace te maken.

[powerbi-client]: https://github.com/Microsoft/PowerBI-Cli

Een bestand kan op twee manieren worden toegevoegd aan de **Workspace Collection**:
1. De [powerbi-client]. Een command-line tool waarmee via commando's een Workspace kan worden aangemaakt of een rapport kan worden geupload naar de workspace.
2. De [Power BI Embedded REST API](https://github.com/Microsoft/PowerBI-Cli). Met de api is verdere integratie van rapport- en workspace-beheer in een maatwerkapplicatie mogelijk.

In ons voorbeeld gebruiken we de [powerbi-client]. De kan worden geinstalleerd via npm.
                   
    npm install powerbi-cli -g

Vervolgens kan er met een aantal commando's eenvoudig een rapport worden geupload.

1. Aanmaken van eeen workspace

       powerbi create-workspace -c <collection> -k <accessKey>

2. Toevoegen van rapport aan aangemaakte workspace

       powerbi import -c <collection> -w <workspaceId> -k <accessKey> -f <file> -n [name] -o [overwrite]

3. Genereren van een embed token

       powerbi create-embed-token -c <collection> -k <accessKey> -w <workspaceId> -r <reportId> -u [username] --roles [roles1,roles2,...] -s [scope1 scope2 ...] -e <expiration>

Het resultaat is:
* een Workspace aangemaakt binnen de Workspace Collection;
* een Rapport geupload naar de Workspace;
* Een embed token die we nodig hebben om het rapport te benaderen.

Met deze gegevens kunnen we nu naar de laatste stap, namelijk het [Rapport integreren in een webpagina].