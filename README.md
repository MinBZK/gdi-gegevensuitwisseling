# Algemeen
Dit is de GitHub repository van de MIDO/GDI werkgroep gegevensuitwisseling. Deze werkgroep is verantwoordelijk voor de (door)ontwikkeling van de domeinarchitectuur gegevensuitwisseling. De nieuwe versie van deze architectuur wordt ontwikkeld in de vorm van een ArchiMate architectuurmodel, die te vinden is in deze repository.

Het architectuurmodel is beschikbaar in verschillende vormen:
1. In de vorm van <a href="gegevensuitwisseling.archimate">een bestand</a> voor het modelleertool Archi;
2. Als bestanden die kunnen worden ingelezen met de coArchi plugin van Archi;
3. Als <a href="https://minbzk.github.io/gdi-gegevensuitwisseling">website</a> in de vorm van een HTML report uit Archi;
4. In pagina's en overzichten die met een script zijn geëxporteerd uit Archi om er op een vriendelijke manier doorheen te navigeren, inclusief <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/Domeinarchitectuur%20gegevensuitwisseling.html">een pagina met een samenvatting van de belangrijkste onderdelen.</a> 

Er zijn <a href="instructies.md">instructies</a> beschikbaar voor het aanbrengen van wijzigingen en het installeren en configureren van Archi. Daarnaast is er een beschrijving van het gehanteerde <a href="metamodel.md">metamodel</a>.

Bij de verschillende onderdelen van de architectuur wordt verwezen naar beschrijvingen, diagrammen, overzichten en detailoverzichten. Deze zijn allemaal geëxporteerd uit het architectuurmodelleertool Archi. De diagrammen zijn onderdeel van de standaard Archi HTML report. Het document als geheel, de overzichten, detailoverzichten en de achterliggende detailpagina's zijn gegenereerd met een <a href="scripts/export HTML.ajs">script</a>.

#Review
Er is een review gestart van de conceptversie van de domeinarchitectuur. Het <a href="https://pgdi.nl/files/view/2b9325a0-c193-4d22-b8d1-9b8224a1606d/domeinarchitectuur-gegevensuitwisseling-1.pdf">document</a>, de bijbehorende <a href="https://pgdi.nl/files/view/d0b1bc35-c48a-4da8-af83-2bcfc1527c1f/toelichting-domeinarchitectuur-gegevensuitwisseling.pptx">toelichtende presentatie</a> en het <a href="https://pgdi.nl/files/view/79e6b3cb-6a14-4c78-95df-9d99e239d9ed/reviewformulier.xlsx">reviewformulier</a> zijn beschikbaar op <a href="https://pgdi.nl/groups/view/7d10e3c4-540d-4b20-ac04-d4011a6a90dc/architectuurraad-en-architectuurwerkgroepen/files/e2c148a1-d036-4a5e-92ff-df3d22da6285">pgdi.nl</a>. De opname van de informatiesessie is beschikbaar op <a href="https://youtu.be/clE9n7EOedo">YouTube</a>. Reviewcommentaar kan worden opgestuurd naar postbus.pgdi@minbzk.nl. De deadline voor de review is 17 juni 9.00 uur.

# Architectuur
Inleiding: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-f763d8baeed7450a801180ca97a5e0bc.html">beschrijving</a>.

Veranderfactoren:
* Ontwikkelingen: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/ontwikkelingen.html">overzicht</a>
* Beleid: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/beleid.html">overzicht</a>
* Wet- en regelgeving: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/wetten.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/wettendetails.html">details</a> 
* Knelpunten: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/knelpunten.html">overzicht</a>
* Capability's: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-c86dd5efc983469aa01d883e87689369">diagram</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/capabilities.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/capabilitiesdetails.html">details</a>

Doelarchitectuur:
* Architectuurvisie: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-65626af39b714343abdc1b5e9d8bfb21.html">beschrijving</a>
* Architectuurprincipes: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-4e701366fd844120b700c114068bc91e">diagram</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/principes.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/principesdetails.html">details</a>
* Verdieping op thema metagegevens: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-b7da2fb1fe314dbfb7d025d2f1a07035.html">beschrijving</a>
* Verdieping op thema communicatieprotocollen: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-1d2d4327d948422eadfcd5208208ec3a.html">beschrijving</a>
* Verdieping op thema historie: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-dcfbaf9541ce478aa0eb2bac5e9fb2dd.html">beschrijving</a>
* Verdieping op thema eventoriëntatie: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-070bf0b5f6884999a5b5b742c8ee6ce5.html">beschrijving</a>
* Veranderinitiatieven: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/veranderinitiatieven.html">overzicht</a>

Bijlagen:
* Functies: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-6b14d70bd65443bfbf08cd9326376898">diagram</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/bedrijfsfuncties.html">overzicht</a>
* Bedrijfsobjecten: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-efc531031d114860a309f6eeacdad289">diagram</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/bedrijfsobjecten.html">overzicht</a>
* Relatie tussen functies en bedrijfsobjecten: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-b6f068818d264742b80c8f4f5278aca0">diagram</a>
* Rollen: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/rollen.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/rollendetails.html">details</a>
* Huidige voorzieningen: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-44e956451b5947e08070f8c2edca5bf3">diagram</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/huidige%20voorzieningen.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/huidige%20voorzieningendetails.html">details</a>
* Standaarden: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/?view=id-5df0c1360768493aa966c16f7dbfd414">diagram</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/standaarden.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/standaardendetails.html">details</a>
* Begrippen: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/begrippen.html">overzicht</a>, <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/begrippendetails.html">details</a>
* Relatie van architectuurprincipes met ADO en NORA: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/elements/id-98a74bf2a0b444ebba06ffda16362eb8.html">overzicht</a>

Documenten:
* Samenvatting van de belangrijkste onderdelen in één pagina: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/Domeinarchitectuur%20gegevensuitwisseling.html">samenvatting</a>
* Bijlagen in één pagina: <a href="https://minbzk.github.io/gdi-gegevensuitwisseling/content/views/Bijlagen%20domeinarchitectuur%20gegevensuitwisseling.html">bijlagen</a>
