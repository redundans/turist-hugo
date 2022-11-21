---
date: 2021-03-28
title:  "Minimal jäskyl för hembryggning på budget"
---
Jag har precis som de flesta som bryggt öl hemma på hobbynivå förstått att det är dags att få kontroll på jästemperaturen om det skall vara värt att fortsätta förbättra min öl.

Jag har turen att kunna nyttja både vindsföråd och potatiskällare för att stundtals hitta en bra jästemperatur. Men den större delen av året är jag ändå rätt begränsad. 

Då jag bor i en rätt mindre lägenhet så är införskaffandet av en jäskyl uteslutet. Jag behöver något som är anpassat till mina små experimentella satser och som jag kan plocka fram endast vid behov.

![brewfather](/assets/images/DSC00621.png)
*Jäskylen kommer kanske inte vara med i någon heminredningstidning precis. Men den fungerar!*

## En jäskyl av en enkel kylväska

Jag bestämde mig helt simpelt för en kombinerad kylbox / värmebox från Biltema. Jag byggde sedan en enkel termostat utav en Arduino Nano och en temperatursensor (DS18B20) som styr om värmen / kylan skall slås på eller av.

Funktionaliteten är enkel. Med hjälp av två knappar stegar man in en SET TEMP som sedan bestämmer om boxen behöver sätta på mer kyla eller mer värme. Temperaturen som mäts i boxen tillåts fluktuera en halv grad + / - SET TEMP.

För att kontrollera temperaturen har jag kopplat in en 1602 LCD-skärm som visar nuvarande temperatur och SET TEMP.

Tanken var också att använda en spännings-regulator för att nyttja boxens 12v för att driva min termostat. Men så länge jag begöver kunna förfina mitt program låter jag USB-kontakten hänga ut, vilken används som strömkontakt.

## Första försöket med US-05

Vid mitt första försök så hade jag bara kopplat en relä som styrde om kylboxen var på eller av. Uppvärmningen efter utjäsning fick skötas i rumstemperatur, innan flaskningen. För extra kontroll lät jag min lilla [iSpindel](https://www.ispindel.de/) ligga i under jäsningen och skicka uppdateringar under hela processen till [Brewfather](https://brewfather.app/).

![brewfather](/assets/images/brewfather.png)
*Jäsdiagram från Brewfather för en American Wheat, jäst med US-05.*

Som ni ser i diagramet ovan så har temperaturen (blå linje) hålt sig hyffsat stabilt strax över 18 grader (vilket var min SET TEMP) under hela jäsningen. Trots att jäsningen var väldigt aktiv i början och antagligen producerade en hel del värme.

Min iSpindle är lite otillförlitlig när det kommer till små satser på ~5 liter, vilket är förståligt då den mäter utjäsning med hjälp av ett gyroskop. Men mätningen med min hydrometer visade på ett OG på ~1.043 och en FG på ~1.008. Vilket var precis enligt plan.

Innan flaskningen så smakade jag av ölen. Krispigt och tämligen ren och jag tyckte mig inte känna några tecken på en stressad jäst. Resultatet kommer förhoppningsvis återspegla mina brister på andra håll än just jästemperaturen denna gån.

### Anpassad jästunna

För att få plats med själva jästunnan så var jag tvungen att hålla mig till kylboxens inre dimensioner (32x21x38 cm). Det enklaste var helt enkelt att köpa en enkel vattendunk med tappkran på fem liter och göra ett hål för jäsventil i locket. Tråkigt att jäsa i plast men det breda locket på vattendunkar gör den i alla fall lätt att rengöra.

## Projektets kostnad

En hel del saker hade jag liggande hemma. Och hade jag inte haft det så hade valet av komponenter sett anorlunda ut (finns ju färdiga 12-voltstermostater för under 200 kr). Men om jag hade köpt allt nytt hade kostnaden nog blivit ungefär såhär:

* Kylbox / värmebox Biltema - 399,00 kr
* ATmega328 5 Volt Arduino nano kompatibel - 67,00 kr
* Digital vattentät temperaturgivare DS18 B20 - 39,00 kr
* Relä 5 Volt 2 kanal - 39,00 kr
* LCD HD44780 Kompatibel 16x2 tecken - 57,00 kr
* 2 Tryckknapp momentan PBS-110 - 58,00 kr
* Vattendunk med tappkran 5 L - 88,63 kr

**Totalt: ~748,00 kr**

---

## Så hur funkar det?

Det hela hade kanske kunnat göras både bättre och billigare. Men jag är rätt nöjd att komma undan med en jäskyl som jag kan gömma undan i en garderob mellan bryggningarna – dessutom för mindre än 800 kr. Suboptimalt är att jag inte nyttjar boxens hela storlek samt ljuder från fläkten som sätts på och stängs av med jämna mellanrum.

En tänkbar uppdatering inför framtiden är att byta ut den termoelektriska kylaren (TEC) till en något vassare modell samt förbättra fläkten för att få kylen tystare.

Hur som helst har jag fått löda, programmera och brygga öl. Och det är ovärdeligt för mig.