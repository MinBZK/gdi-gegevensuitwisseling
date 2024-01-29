# Installeren en configureren Archi

## Voor lezers
1. Installeren Archi: https://www.archimatetool.com/download/
2. Downloaden ArchiMate bestand: https://github.com/MinBZK/gdi-gegevensuitwisseling/blob/master/gegevensuitwisseling.archimate
3. Inlezen ArchiMate bestand in Archi (File>Open)

## Voor mensen die wijzigingen willen aanbrengen
1. Downloaden coArchi: https://www.archimatetool.com/downloads/coarchi/coArchi_0.9.0.archiplugin
2. Installeren coArchi in Archi (Help>Manage Plug-ins, en dan Instal New...)
3. Aanmaken Github account
4. Genereren Personal Access Token in GitHub: (Settings>Developer settings>Personal access tokens>Tokens (classic))
5. Clonen repository met een github client (bijvoorbeeld https://desktop.github.com/): https://github.com/minbzk/gdi-gegevensuitwisseling
6. Importeren model in Archi (Collaboration>Import Remote Model To Workspace) met URL: https://github.com/minbzk/gdi-gegevensuitwisseling, Personal Access Token als wachtwoord
7. Open repository in Archi door dubbelklikken op de naam van de repository in de Collaboration Workspace
8. Downloaden jArchi: https://www.archimatetool.com/plugins/, kleine donatie noodzakelijk
9. Installeren jArchi in Archi (Help>Manage Plug-ins, en dan Instal New...)
10. Kopiëren script naar scripts folder van Archi: https://github.com/MinBZK/gdi-gegevensuitwisseling/blob/master/scripts/export%20HTML.ajs

## Voor repository beheerders
1. Aanpassen script aan metamodel van repository: https://github.com/MinBZK/gdi-gegevensuitwisseling/blob/master/scripts/export%20HTML.ajs, variabelen relationshipTypeMappings, elementTypeMappings, elementTypePluralMappings en elementTypes

# Aanbrengen van wijzigingen
1. Wijzigingen in Archi committen (Collaboration>Commit Changes) 
2. Wijzigingen in Archi publiceren (Collaboration>Publish Changes)
3. Genereren HTML report in Archi (File>Report>HTML), met als doeldirectory de docs directory op de lokale clone van de repository
4. Genereren aanvullende HTML pagina's voor overzichten met script (Scripts>export HTML na het klikken op de naam van de repository, linksnboven in de treeview met de rechtermuisknop), met als doeldirectory de docs/content directory op de lokale clone van de repository
5. Opslaan .archimate bestand in de root directory van de lokale clone van de repository (File>Save As)
6. Sluiten repository (File>Close Model)
7. Heropenen repository in Archi door dubbelklikken op de naam van de repository in de Collaboration Workspace
8. Committen repository in lokale github client
9. Publiceren repository in lokale github client

