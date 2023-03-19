---
{"dg-publish":true,"permalink":"/sekundaerminne/","tags":["datorteknik"]}
---

En sorts [[Computer Data Storage\|minne]] som till skillnad från [[Primärminne\|Primärminne]] behåller sitt innehåll när strömmen slås av. Det är alltså inte flyktigt (non-volatile). Exempelvis hårddisk, flashminne, magnetband, cd, dvd etc.

I en hårddisk flyttas ett läs och skrivhuvud för att läsa önskad data, vilket är långsamt.

Minnet är uppdelat i cluster av en viss storlek. Om man vill lagra en fil får den ofta inte plats i ett cluster, utan [[Fragmentering\|fragmenteras]] till olika delar. 

Man använder inte bara närliggande cluster som kommer efter varandra, för om man har olika stora filer som ska lagras är det inte säkert att alla får plats även om det finns ledigt utrymme (extern [[Fragmentering\|fragmentering]]).

Ett alternativ är en länkad lista. Extern [[Fragmentering\|fragmentering]] försvinner och man kan lagra stora filer, men för att hämta något i slutet av en fil måste hela filen sökas igenom. 

Ett annat alternativ är att ha ett block som innehåller pekare till alla fragment. Extern [[Fragmentering\|fragmentering]] försvinner, men lagringen är begränsad till det antal pekare som får plats i ett block.

Ännu ett är Inode (som används i Unix). Inode har några pekare som pekar direkt på block, men den har även pekare som pekar på ett block med pekare osv.

# Partitioning
När man delar in en fysisk hårddisk i en eller flera logiska hårddiskar.