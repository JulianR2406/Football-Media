# Mediennetzwerke der Profi- und Amateurfußballvereine in Baden-Württemberg
# Datensatz
Codebuch Mediennetzwerke Profi- und Amateurfußball BW 
Stand Abgabe (17.1.2025)

Erstellt von Julian Rebmann (jr126)

## Inhalt
- footballmedia_edges.csv (Edgelist)
- footballmedia_nodes.csv (Nodelist)
- Codebuch Footballmedia.md (Codierung der Datensätze)

## Ursprung und Datenerhebung
Der Ursprung meiner Forschung liegt im Rahmen meiner Bachelorarbeit im Studium Crossmedia-Redaktion/Public Relations an der Hochschule der Medien in Stuttgart. 

Der Datenzugang erfolgt über die Websites und Social-Media-Auftritte der 14 untersuchten Vereine sowie verschiedener Newsportale, Interviews und Mailanfragen an die Vereine. 

Das Netzwerk ist ein *ungerichtetes Gesamtnetzwerk*. 

# EDGELIST-Attribute

**from**  
Entspricht den IDs der Vereine, Verbände und Verlagshäusern / Mediengruppen in der Nodelist.

**to**  
Entspricht der ID der Medienpartner oder der Vereine

**weight**  
Definiert die Art der Geschäftsbeziehung: 1 = rechtliche Beziehung (gehört zusammen), 2 = offizielle Partnerschaft, 3 = inoffizielle Partnerschaft (Zusammenarbeit) oder Fan-Medium, 4 = regelmäßige Berichterstattung (Verein), 5 = unregelmäßige Berichterstattung (liga-basiert)

**liga**
Entspricht der Ligazugehörigkeit des Vereins in der Saison 2024/25: eins, zwei, drei, vier

**category**
Entspricht den Kategorien der Vereine: pro (Erst- und Zweitligisten), ama (Dritt- und Viertligisten)

# NODELIST-Attribute  
  
**id**  
Eindeutige Identifikation der einzelnen Knotens (Vereine, Verbände, Medien), der erfasst wird.  

**name**  
Name des Verbands, des Vereins oder des Mediums als klare Bezeichnung des Knotens. 

**type**  
Art des Knotens: medium, verein, verband

**liga**   
Ligazugehörigkeit der Vereine: eins, zwei, drei, vier, bei Medium und Verband bleibt diese Zeile leer.

**rechtsform**   
Rechtsform der Vereine: GmbH, EV, AG, bei Medium und Verband bleibt diese Zeile leer.

**media**             
Art der Medien: TV, Radio, Zeitung, Streaming, Gaming, Druck, Werbung, PR Marketing, Film und Foto, Website, Blog, Verlag, bei Verein und Verband bleibt diese Zeile leer.

**reichweite**
Reichweite/Zielgruppe der Medien: GER (Deutschland/überregional), BW (ganz Baden-Württemberg), Region (regional), VFB (Fanangebot des VfB).
