# Algemeen
Dit is de GitHub repository van de MIDO/GDI werkgroep gegevensuitwisseling. Deze werkgroep is verantwoordelijk voor de (door)ontwikkeling van de domeinarchitectuur gegevensuitwisseling. De nieuwe versie van deze architectuur wordt ontwikkeld in de vorm van een ArchiMate architectuurmodel, die te vinden is in deze repository. 

Het architectuurmodel is beschikbaar in verschillende vormen:
1. In de vorm van <a href="gegevensuitwisseling.archimate">een bestand</a> voor het modelleertool Archi
2. Als bestanden die kunnen worden ingelezen met de coArchi plugin van Archi
3. Als <a href="https://minbzk.github.io/gdi-gegevensuitwisseling">website</a> in de vorm van een HTML report uit Archi
4. In pagina's en overzichten die met een script zijn geëxporteerd uit Archi om er op een vriendelijke manier doorheen te navigeren (zie hieronder)

# Diagrammen en overzichten
De volgende diagrammen en overzichten zijn geëxporteerd uit Archi. De diagrammen zijn onderdeel van de standaard Archi HTML report. De overzichten en achterliggende detailpagina's zijn gegenereerd met een <a href="scripts/export HTML.ajs">script</a>.

## Diagrammen
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/id-06c6c1de430644b9adb865225da06cba/views/id-f7226f7c68704aae807b71a2f10b1cce.html">Functiemodel</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/id-06c6c1de430644b9adb865225da06cba/views/id-efc531031d114860a309f6eeacdad289.html">Bedrijfsobjectenmodel</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/id-06c6c1de430644b9adb865225da06cba/views/id-b6f068818d264742b80c8f4f5278aca0.html">Functiemodel met bedrijfsobjecten</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/id-06c6c1de430644b9adb865225da06cba/views/id-750e714e84f54659ac784d7e040b4629.html">Architectuurprincipes</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/id-06c6c1de430644b9adb865225da06cba/views/id-5df0c1360768493aa966c16f7dbfd414.html">Standaarden</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-44e956451b5947e08070f8c2edca5bf3">Huidige voorzieningen</a>

## Overzichten
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/bedrijfsfuncties.html">Functies</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/bedrijfsobjecten.html">Bedrijfsobjecten</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/principes.html">Architectuurprincipes</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/standaarden.html">Standaarden</a>
* <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/voorzieningen.html">Huidige voorzieningen</a>

# Instructies

## Aanbrengen van wijzigingen
Als iemand wijzigingen aanbrengt in het model dan moet er door deze persoon ook een nieuwe HTML export worden gemaakt en gepubliceerd alsook een export van het toegang.archimate bestand. Voor de HTML export moet een HTML report worden gegenereerd met Archi en moet daarnaast het <a href="scripts/export HTML.ajs">script</a> worden uitgevoerd om de aanvullende overzichten en detailpagina's te genereren.

## Installeren en configureren coArchi
1. Installeren Archi: https://www.archimatetool.com/download/
2. Installeren coArchi: https://www.archimatetool.com/downloads/coarchi/coArchi_0.9.0.archiplugin
3. Aanmaken Github account
4. Genereren Personal Access Token: Settings/Developer settings/Personal access tokens/Tokens (classic)
5. Import Remote Model To Workspace in Archi: URL: https://github.com/minbzk/gdi-gegevensuitwisseling, Personal Access Token als wachtwoord

