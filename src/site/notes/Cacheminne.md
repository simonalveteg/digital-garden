---
{"dg-publish":true,"permalink":"/cacheminne/","tags":["datorteknik"]}
---

![Pasted image 20230215152134.png](/img/user/images/Pasted%20image%2020230215152134.png)

Det kostar tid att ladda in något till cache-minnet, men om de ska användas igen går det mycket snabbare att lässa från cacheminnet än det hade gjort att läsa från primärminnet.

Minnesreferenser tenderar att gruppera sig under exekvering, det kallas lokalitet av referenser. 

Cacheminnet är kopplat till CPUn och används för att få ett minnessystem som verkar både stort och snabbt. För det utnyttjar man lokalitet genom att kopiera "recently accessed (and nearby) items" från hårddisken till mindre primärminne, sedan kopieras mer "recently accessed (and nearby) items" från primärminnet till cacheminnet. 

# Direct mapped cache
Data kan hamna på ett ställe i cacheminnet. Eftersom att primärminnet är mycket större än cacheminnet kommer data från flera olika adres,ser mappas till samma adress i cacheminnet. Om det redan finns data på den platsen i cacheminnet kommer den att skrivas över med den nya. 

De blå adresserna i minnet nedan mappar till den blå adressen i cacheminnet.
![Pasted image 20230215153704.png](/img/user/images/Pasted%20image%2020230215153704.png)
alternativ:
![Pasted image 20230215153835.png](/img/user/images/Pasted%20image%2020230215153835.png)
Direct mapped är en enklare design men mindre flexibel. Fully associative är mer flexibelt men även mer komplext - det tar längre tid att hitta datan i cacheminnet.

# Skrivstrategier

## Write-through
Skrivningar i cache görs också direkt i primärminnet. 

## Write-through with buffers
Skrivningar buffras och görs periodiskt

## Write (Copy)-back
primärminnet uppdateras först när en cacherad byts ut (ofta används en bit som markerar om en cacherad blivit modifierar (dirty))

# Cachenivåer
Man kan ha olika nivåer av cacheminnen.

Man kan även ha separat cacheminne för minne och instruktioner.