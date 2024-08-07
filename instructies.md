# Installeren en configureren Archi

## Voor lezers
1. Installeren Archi versie 5.2.0: https://www.archimatetool.com/download/ 
2. Downloaden ArchiMate bestand
3. Inlezen ArchiMate bestand in Archi (File>Open)

## Voor mensen die wijzigingen willen aanbrengen
1. Zeker stellen dat je versie 5.2.0 van Archi gebruikt (hiermee is het script getest) en anders deze versie downloaden en installeren
2. Downloaden coArchi: https://www.archimatetool.com/downloads/coarchi/coArchi_0.9.0.archiplugin
3. Installeren coArchi in Archi (Help>Manage Plug-ins, en dan Install New...)
4. Aanmaken GitHub account
5. Genereren Personal Access Token in GitHub: (Settings>Developer settings>Personal access tokens>Tokens (classic))
6. Clonen repository met een GitHub client (bijvoorbeeld https://desktop.github.com/)
7. Importeren model in Archi (Collaboration>Import Remote Model To Workspace), met Personal Access Token als wachtwoord
8. Open repository in Archi door dubbelklikken op de naam van de repository in de Collaboration Workspace
9. Downloaden jArchi: https://www.archimatetool.com/plugins/, kleine donatie noodzakelijk
10. Installeren jArchi in Archi (Help>Manage Plug-ins, en dan Install New...)
11. Kopiëren script naar scripts folder van Archi: https://github.com/MinBZK/gdi-gegevensuitwisseling/blob/master/scripts/export%20HTML.ajs

## Voor repository beheerders
1. Aanpassen script aan metamodel van repository: https://github.com/MinBZK/gdi-gegevensuitwisseling/blob/master/scripts/export%20HTML.ajs, variabelen relationshipTypeMappings, elementTypeMappings, elementTypePluralMappings en elementTypes, of overleggen of generieke script aangepast kan worden
2. Kopiëren van https://github.com/MinBZK/gdi-gegevensuitwisseling/blob/master/docs/js/frame2.js naar de /docs/js directory van de repository.
3. Aanmaken van specialisaties voor repository in Archi conform <a href="metamodel.md">metamodel</a> (Tools>Specializations Manager)

# Aanbrengen van wijzigingen
1. Wijzigingen in Archi committen (Collaboration>Commit Changes) 
2. Wijzigingen in Archi publiceren (Collaboration>Publish Changes)
3. Genereren HTML report in Archi (File>Report>HTML), met als doeldirectory de docs directory op de lokale clone van de repository
4. Genereren aanvullende HTML pagina's voor overzichten met script (Scripts>export HTML, na het klikken op de naam van de repository, linksboven in de treeview met de rechtermuisknop), met als doeldirectory de docs/content directory op de lokale clone van de repository
5. Opslaan .archimate bestand in de root directory van de lokale clone van de repository (File>Save As)
6. Sluiten repository (File>Close Model)
7. Heropenen repository in Archi door dubbelklikken op de naam van de repository in de Collaboration Workspace
8. Committen repository in lokale GitHub client
9. Publiceren repository in lokale GitHub client

De volgende specifieke aandachtspunten gelden bij het maken van ArchiMate modellen:
* Gebruik alleen elementen zoals gedefinieerd in het <a href="metamodel.md">metamodel</a> 
* Gebruik de in het <a href="metamodel.md">metamodel</a> voorgedefinieerde specialisaties, en voor alle andere modelelementen expliciet geen specialisatie
* Gebruik de eigenschappen zoveel mogelijk zoals ook gehanteerd in het standaard <a href="metamodel.md">metamodel</a>
* Definieer voor alle modelelementen die niet door het script in de standaard HTML lijsten gegenereerd moeten worden een eigenschap "exclude" zonder waarde
