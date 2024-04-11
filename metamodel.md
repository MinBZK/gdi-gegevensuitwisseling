# Metamodel MIDO/GDI domeinarchitecturen

<img src="https://minbzk.github.io/gdi-gegevensuitwisseling/images/metamodel.svg">

* Architectuurprincipe
	- ArchiMate type: Principle
	- Name: stelling van het principe, voorafgegaan door een volgnummer, een punt en een spatie (eventueel hiërarchisch)
    - Documentation: rationale
	- Implicaties: per implicatie, waarbij elke implicatie start met een volgnummer, een punt en een spatie
	- Influence: Wetgeving die wordt ondersteund door het principe
* Begrip
	- ArchiMate type: Meaning
	- Name: voorkeursterm voor het begrip, startend met een kleine letter
	- Documentation: definitie
	- ID: gelijk aan naam (relevant voor het voorkomen van dubbelingen bij opnieuw importeren)
	- Eigenschappen uit <a href="https://profielstelselcatalogus.pldn.nl/">NL-SBB standaard</a> zoals Toelichting
* Bedrijfsfunctie
	- ArchiMate type: Business Function
	- Name: korte duiding van de bedrijfsfunctie
	- Documentation: definitie van de functie in één zin
	- Access: bedrijfsobjecten die worden gebruikt, alleen voor functies op het hoogste niveau
	- Association: architectuurprincipes die hieraan zijn gerelateerd
	- Composition: bedrijfsfuncties die onderdeel uitmaken van de bedrijfsfunctie, alleen voor functies op het hoogste niveau
	- Realization: capabilities die worden ondersteund door de bedrijfsfunctie
* Bedrijfsobject
	- ArchiMate type: Business Object
	- Name: korte duiding van het bedrijfsobject
	- Documentation: definitie van begrip waar het op gebaseerd is
	- Association: bedrijfsobjecten die zijn gerelateerd aan het bedrijfsobject
	- Association: standaarden die gebruikt maken van gegevens die zijn gerelateerd aan het bedrijfsobject
* Beleid
	- ArchiMate type: Driver
	- Name: korte duiding van het beleid
    - Specialization: Beleid
	- Documentation: omschrijving
	- URL: link naar de formele publicatie
* Capability
	- ArchiMate type: Capability
	- Name: korte duiding van de capability
	- Documentation: omschrijving van de capability in één zin die start met "Overheidsorganisaties kunnen ..."
	- Realization: wetgeving die ten grondslag ligt aan de capability 
* Document
	- ArchiMate type: Representation
	- Specialization: Document
	- Name: titel van document
	- Association: pagina die deel uitmaakt van document
		- naam: nummer van de paragraaf in het document
		- nummer: volgnummer die de volgorde in het document beschrijft, startend bij 1, is optioneel
		- niveau: het niveau van de heading (een niveau van 1 == leidt tot de HTML heading H1), als deze niet is gedefinieerd dan wordt er geen heading gegenereerd
		- type: als het een verwijzing naar een elementType is dan "overzicht", "properties" of "details" voor het type overzicht
* Gewenste voorziening
	- ArchiMate type: Application Component
	- Name: korte duiding van de gewenste voorziening
	- Specialization: Gewenste voorziening
	- Documentation: omschrijving
	- Serving: bedrijfsfuncties die worden ondersteund door de voorziening
	- Association: veranderinitiatief dat invulling geeft aan gewenste voorziening
	- Flow: voorziening die gegevens ontvangt van deze voorziening
* Huidige voorziening
	- ArchiMate type: Application Component
	- Name: korte duiding van de huidige voorziening
	- Specialization: Huidige voorziening
	- Documentation: omschrijving
	- Beheerorganisatie: naam van de organisatie die de voorzienint beheert
	- URL: link naar pagina met details over de voorziening, liefst bij de beheerder van de voorziening
	- Serving: bedrijfsfuncties die worden ondersteund door de voorziening
	- Flow: voorziening die gegevens ontvangt van deze voorziening
* Knelpunt
	- ArchiMate type: Assessment
	- Name: korte duiding van het knelpunt
	- Documentation: omschrijving
	- Association: veranderinitiatief dat oplossing biedt voor knelpunt
* Ontwikkeling
	- ArchiMate type: Driver
    - Specialization: Ontwikkeling
	- Name: korte duiding van de ontwikkeling
	- Documentation: omschrijving
* Standaard
	- ArchiMate type: Constraint
    - Specialization: Standaard
    - Name: korte duiding van de standaard
	- Documentation: omschrijving
	- Status: status van de standaard bij Forum Standaardisatie (Verplicht of Aanbevolen) of nvt indien de standaard niet op de lijsten van het Forum Standaardisatie staan
	- Beheerorganisatie: naam van de organisatie de de standaard beheert (overnemen van Forum Standaardisatie indien mogelijk)
	- Functioneel toepassingsgebied: indien gedefinieerd door Forum Standaardisatie deze overnemen, anders weglaten
	- URL: link naar pagina over de standaard bij Forum Standaardisatie in dien mogelijk, anders link naar andere pagina met details over de standaard, liefst bij de beheerder van de standaard
	- Aggregation: standaarden die onderdeel uitmaken van de standaard, vooral bedoeld voor samengestelde standaarden gedefinieerd door Forum Standaardisatie
* Tekst
	- ArchiMate type: Representation
	- Specialization: Tekst
	- Name: titel van pagina
	- Documentation: HTML van pagina	
	- elementType: de naam van het elementtype (inclusief specialisatie) in geval het een verwijzing is naar een overzicht of detailoverzicht
* Veranderinitiatief
	- ArchiMate type: Work Package
    - Name: korte duiding van het Veranderinitiatief
	- Documentation: omschrijving 	
* Wetgeving
	- ArchiMate type: Driver
    - Specialization: Wetgeving
    - Name: korte duiding van de wetgeving
	- Documentation: korte omschrijving 
	- URL: link naar de formele publicatie
