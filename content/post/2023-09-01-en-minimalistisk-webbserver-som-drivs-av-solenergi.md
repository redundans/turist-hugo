---
date: 2023-09-01
title:  "En minimalistisk webbserver som drivs av solenergi"
---
Allt sedan jag läste **Kris De Deckers** ursprungliga bloggpost på [Low-tech magazine](https://solar.lowtechmagazine.com/) om deras soldrivna webbserver har jag haft en idé om att bygga en själv.

Idag drivs den välbesökta bloggen helt på solenenergi och ett helt gäng av kunniga personer har varit inolverade i att få det att fungera så bra som möjligt. Den gamla bloggen har de slutat att uppdatera.

Mitt projekt skiljer sig något från gängets på Low-tech magazine då det är mycket mindre ambitiöst. Jag har försökt att bygga allt med saker som jag redan hade tillgång till eller genom billigaste möjliga inköp.

**Min webbserver består av följande:**

* 50 watt solpanel i monokristallin
* Regulator LS1024EU
* 12 volts AGM-batteri, 7,2 Ah
* Kablar
* Raspberry Pi Zero W

Raspberry:n hade jag sedan tidigare, liksom solpanelen. Alla kablar har jag hämtat från grovsoporna, tvättat och strippat. Eftersom jag är osäker på mitt behov av batteri nöjde jag mig med ett på 7.5 Ah som var tillfälligt på rea. Regulatorn är den billigaste jag kunde hitta som erbjöd 5 watt elförsörjning via USB. Så jag kan driva Raspberry:n direkt från den och slipper skaffa någon typ av power shell för batteridrift.

Mjukvarumässigt så har jag också gjort det lätt för mig. Raspberry:n kör Raspberry OS Lite, Debian 11 (bullseye). För att minska energiåtgången har jag har stängt av HDMI, Bluetooth och en USB-port. Med hänsyn till min sambo använder jag idag tyvärr WIFI för att prata med min router istället för att dra ethernetkablar över hela vår boyta.

Bloggen i sig består av statisk HTML utan länkade assets för att minska både mängden data och requests till servern. Jag är lite osäker på om gzip-komprimering av trafiken skulle ge några energifördelar. Då komprimeringen antagligen kräver mer prestanda än leveransen av data mot internet.

Eftersom serven bor hemma hos mig i stadsnätet utan fast IP så använder jag dessutom en tunnel via Cloudflare (ja, jag vet!) för att man skall kunna nå servern från Internet.

## Problem

Ja, det största problemet är väl att webbservern plötsligt slocknar i brist på energi från batteriet. Men det är en anpassning jag tycker är rimligt. Om någon typ av omställning till hållbar energi skall göras kanske vi måste vänja oss vid att allt inte går att drifta hela tiden och när som helst. Detta är dessutom en blogg och inte ett journalsystem hos akutsjukvården.

Ett annat problem är givetvis kostnaden. Att få till en sån här setup kostar trots att jag snålat över tusen kronor. Tidigare låg bloggen hos GitHub Pages och det var helt "gratis" och hade en upptid på 99%.

## Förbättringar

Det finns många förbättringar att göra. Troligtvis kommer inte solpanelen på 50 watt och ett batteri på 7.5 Ah räcka under de mörkare månaderna här i Sverige. Kanske måste jag utöka energiinsamlingen med större solpaneler eller vindkraft för den blåsiga senhösten. Fortsatt optimering genom att ansluta servern med ethernet och dessutom kunna stänga av WIFI-kretsen från Rasperry:n är också önskvärd.

Dessutom skulle jag vilja köpa en enkel voltsensor och en konverterare mellan analogt och digitalt för att kunna mäta batteriets kapacitet direkt från Raspberry:n. Och dessutom kanske någon typ av power shell som kan sätta servern i periodisk vila under mindre soliga perioder.

---

Det var väl allt jag hade att säga om detta. Under kommande veckor skall jag försöka mäta upptid och göra lite beräkningar på var mitt projekt brister. Har ni några åsikter eller frågor så kontakta mig på Mastodon [indieweb.social/@httpster](https://indieweb.social/@httpster). 