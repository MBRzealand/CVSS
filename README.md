# CVSS opgave


## Afprøvning af CVSS Score calculator
Jeg vil tage udgangspunk i følgende [sårbarhed](https://www.cvedetails.com/cve/CVE-2021-30481/).

Sårbarheden omhandler Gaming-platformen Steam, hvor brugere køber adgang til spil og software. Sårbarheden er formentlig patchet på nuværende tidspunkt da den eksisterede i 2021, men fungerer stadig fint som eksempel til opgaven. Sårbarheden er ikke synderligt veldokumenteret, så både scope og konsekvens er svært at vurdere. Hvad er oplyst om sårbarheden er at hvis en brugere har installeret et Source engine spil, kan "remote authenticated" brugere eksekvere arbitrær kode grundet et buffer overflow som sker i forbindelse med at invitere folk til spillet. 

Alt afhængigt af hvordan Steam-platformen fungerer, kan arbitrær kode-eksekvering medføre evt. gratis køb af spil/software/virtuelle genstande. Disse kan ligeledes videresælges eller videregives til andre brugere. Dette ville derfor være ekstremt slemt fra et virksomhedsstandpunkt. Ligeledes ville man sagtens kunne forestille sig at det ville medvirke til enten tab eller ændring af data på platformen.

Vector string: ```CVSS:3.1/AV:N/AC:H/PR:L/UI:R/S:C/C:H/I:H/A:H/E:F/RL:U/RC:R```

## Anvendelse af cvedetails.com
En af de smarte ting ved hjemmesiden er at den giver et dags- uge- eller månedsoverblik, over hvilke sårbarheder er dokumenterede. Heraf kan man orientere sig om det aktuelle trusselsbillede.  

![image](https://github.com/MBRzealand/CVSS/assets/70659124/4348a094-5522-44e3-88f2-2557cb9194f8)  


foruden dette har siden en søgefunktion der tager imod både produkter samt CVE-numre således man enten kan holde sig opdateret omkring et specifikt produkts sårbarheder, eller undersøge en konkret sårbarhed for at prøve finde information eller deciderede løsninger.

cvedetails.com kan essentielt anvendes som én kæmpe risiko-analyse for samtlige kendte exploits. Alle exploits er dokumenterede og rangerede efter parametre der medvirker til at vurdere hvor svært exploitet er at afvikle, konsekvensen af exploitet, samt hvorvidt exploitet stadig udgør en trussel. Disse parametre forkortes derefter til en "Vector string", som essentielt er en forkortelse for hvad de forskellige vurderingsparametre er vurderet til. CVSS-numre kan deraf anvendes af diverse IT-sikkerheds specialister til at udtrykke deres specifikke risikovurdering af et exploit.  

![image](https://github.com/MBRzealand/CVSS/assets/70659124/04f58ff8-28c0-4e53-82af-675f1b482b3f)

Heraf kan vi altså se hvordan forskellige sikkerhedsaktører har trusselsvurderet det givne exploit. 
