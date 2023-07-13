---
date: 2023-07-13
title:  "Meta's Threats"
---
Under juni månad kom nyheten att företaget bakom Instagram och Facebook, **Meta Platforms, Inc**, skulle lansera en ny produkt.

Produkten som heter **Threads** skulle använda sig av protokollet [ActivityPub](https://activitypub.rocks/) för att kommunicera med andra tjänster och eventuellt andra instanser av Threads på Internet.

Detta slog ned som en bomb i det som slarvigt kallas fediversum. Jag förstod inte riktigt varför – och framför allt inte varför tonläget bland de som hade skilda åsikter om Metas närvaro på det federerade Internet var så högt (läs otrevligt).

Under början av juli månad försökte jag sätta mig ned och läsa det som skrivits om ämnet (eller snarare det jag hittat om ämnet) för att få en bättre förståelse.

Detta är min sammanfattning.

## Företaget Meta Platforms, Inc

Företaget Meta Platforms, Inc omsätter väldigt mycket pengar. Majoriteten av dessa pengar kommer från  handeln med reklam. Alla deras produkter erbjuder reklamplats och betalt innehåll riktat mot sina användare.

Ibland hör man folk påstå att "i sociala medier är det du som är produkten". Detta är på många sätt sant. Hårdvalutan på reklammarknaden är välriktade reklamutrymmen. För att kunna erbjuda det försöker Meta veta allt om sina användare (och icke-användare). En stor del av Metas verksamhet består därför av massövervakning.

Det är därför inte helt främmande att tänka sig att allt som Meta tar i också i framtiden kommer att förvandlas en vidrig smet av reklam och övervakning.

## Vad är ens fediversum?

En diskrepans i debatten kan nog härledas till att folk tycks ha helt olika uppfattning om vad fediversum egentligen är för någonting. Eller snarare vad fediversum har potential att bli och att erbjuda i framtiden.

För enkelhetens skull kan vi dela upp dessa åsikter i två kategorier:

- **1** Fediverse är designsystem för ett öppet internet
- **2** Fediverse är en social motkultur

Den första gruppen fokuserar oftast på kommunikationsteknik i allmänhet och på protokoll som ActivityPub i synnerhet. Medan den andra gruppen framför allt intresserar sig för social organisering på internet i allmänhet och på Mastodon i synnerhet.

>> "Fediversum är ett nätverk av olika webbtjänster och -servrar som kommunicerar över en uppsättning gemensamma protokoll." - [Wikipedia](https://sv.wikipedia.org/wiki/Fediversum)

Oavsett vilket läger man känner sig hemma i kan man konstatera att ActivityPub ≠ Mastodon samtidigt som man kan vara en förespråkare av både förekomsten av designsystem för ett öppet internet och sociala motkulturer.

## Strategier mot Meta

Oavsett vilket läger folk representerar i debatten så verkar samtliga kritiska till Metas intåg i fediversum. Även om synen på motstrategier knappast är samstämmig. Varken inom grupperna eller mellan dem.

**vantablack** (@vantablack@beach.city) har skapat en pakt ([Anti-Meta Fedi Pact](https://fedipact.online/)) som riktar sig till moderatorer och administratörer för instanser i fediversum som lovar att blocka Metas servrar så fort de börjar använda protokollet ActivityPub.

Andra, som t.ex. **Tim Chambers** (@tchambers@indieweb.social), som är administratör för den instans (indieweb.social) som jag bor på, har valt en mer försiktigt policy:

>> "Don't preemptively strike meta w/ a fediblock, but stay vigilant with eyes wide open and a finger on the block button”. - [Tim Chambers](https://indieweb.social/@tchambers/110568723404841278)

[Jon](https://privacy.thenexus.today/should-the-fediverse-welcome-surveillance-capitalism/) som skrivit det utmärkta inlägget *Should the Fediverse welcome its new surveillance-capitalism overlords? Opinions differ!* delar upp dessa strategier i två kategorier:

- **A** Preemptively block
- **B** Trust but Verify

## En matris av åsikter

För att fördumma debatten en aning och samtidigt hjälpa mig att förstå de olika hållningarna till motstrategier så ritade jag upp en fyrfältare. Här ryms alltså en kombination av de två olika grupperna och de två olika strategierna samtidigt.

![fyrfaltare](/fyrfaltare.svg)

**1A** argumenterar för att Metas intåg i fediversum riskerar att döda öppna designsystem genom att använda dem för massövervakning och spammande av reklam. ActivityPub har idag inget närmare stöd för privat integritet, ”networks of consent” osv. Om detta missbrukas av Meta riskerar de som bryr sig om dessa frågor att vända sig till proprietär mjukvara.

**2A** tycks istället, likt vantablack argumenterar, vilja skydda sina medmänniskor och gemenskaper. På flera instanser av Mastodon har det under flera års tid växt fram en motkultur mot den racism, antisemitism, misogyni samt trans- och homofobi som florerar på just de tjänster som ägs av Meta. Att preventivt blocka Meta är en strategi för att bevara denna motkultur.

**1B** tycker att massblockning av det här slaget går emot själva idéen med ett öppet internet. Alla skall (i stort sätt) kunna kommunicera med alla. Och med denna preventiva blockning hålls miljoner av människor isär från varandra.

**2B** drivs i mångt och mycket av samma grundargument som 2A men menar att det är Meta som har mest att riskera genom att öppna dörren gemenskaper som har mycket mer att erbjuda sina deltagare än vad Meta har. Tack vare att konton lätt (nåja) kan flyttas mellan instanser hoppas man att Metas användare skall förflytta sig till instanser på Mastodon som drivs av sundare värderingar.

## Mina personliga åsikter

Threads är nu släppt och jag har inte ens varit i närheten av den. Andra har dock sammanfattat sina erfarenheter:
- https://www.admdnewsletter.com/p/threads-mastodon-and-the-loneliness
- https://www.zdnet.com/article/ive-used-social-networks-since-the-80s-threads-is-the-most-annoying-one-ive-tried/
- https://www.vice.com/en/article/epvp8j/threads-is-all-the-worst-parts-of-twitter-and-instagram-in-one-very-bad-app

Jag inte heller ngon klar åsikt om vilken strategi fediversum skall anamma. [Kamratadatföreningen Konstellationen](https://konstellationen.org/) som jag också är medlem i har just nu en omröstning bland sina medlemmar om hur [social.Spejset](https://social.spejset.org/) (Mastodon-instansen vi förvaltar) skall förhålla sig i frågan. Men eftersom jag personligen bor på en annan instans kommer jag nog lägga ned min röst i frågan.

Många konstaterar också att en block av Metas instanser inte är något skydd mot deras övervakning. ActivityPub erbjuder inget sådant skydd och Meta har varit notoriskt duktiga på att övervaka sådant som sker på det öppna internet.

Samtidigt tycker jag att debatten om Metas intåg i fediversum lärt mig väldigt mycket om fediversums typografi, teknologi och de olika motkulturer som bor där. Och jag tror inte att jag är ensam om denna upplevelse.

## Merläsning

- https://www.cacherules.com/blog/2023/6/resistance-is-futile-you-will-be-assimilated-by-meta
- https://about.scicomm.xyz/doku.php?id=blog:2023:0625_meta_on_the_fediverse_to_block_or_not_to_block
- https://darnell.day/facebook-fears-the-fediverse
- https://privacy.thenexus.today/should-the-fediverse-welcome-surveillance-capitalism/
- https://ploum.net/2023-06-23-how-to-kill-decentralised-networks.html
- https://ianbetteridge.com/2023/06/21/meta-and-mastodon-whats-really-on-peoples-minds
- https://indieweb.social/@tchambers/110568723404841278
- https://heat-shield.space/mastodon_two_camps.html
- http://wok.oblomov.eu/tecnologia/credible-threat-1/
- https://heat-shield.space/mastodon_two_camps.html
- 