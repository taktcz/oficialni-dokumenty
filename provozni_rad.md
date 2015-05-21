Provozní řád vpsFree.cz, z.s.
=============================

Obsah
-----

0. Vymezení a platnost dokumentu
1. Definice prostředků dostupných členům
2. Základní pravidla při manipulaci se svěřenými prostředky
3. Postupy proti členům narušujícím provoz


0. Vymezení a platnost dokumentu
--------------------------------

1. Provozní řád upravuje zejména parametry prostředků dostupných členům spolku
vpsFree.cz ("Spolek"), šíře kompetencí delegovatelných do provozního řádu je
definována ve stanovách Spolku.

2. Tato verze vstupuje v platnost 1. 7. 2015

1. Definice prostředků dostupných členům
----------------------------------------

### Základní definice

1. Základními prostředky v rámci infrastruktury Spolku se rozumí:
  1. Virtuální server (VPS) je OpenVZ kontejner o parametrech:
    - 8 jader CPU,
    - 4 GB RAM,
    - 60 GB diskového prostoru,
    - 1 veřejná IPv4 a IPv6 adresa
    - Konektivita podle lokace; VPS umístěný v DC Praha je omezené QoS
      mechanismem na maximální propustnost 300 Mbps half-duplex, 600 Mbps
      full-duplex; měsíční limit přenosů VPS v Praze je stanoven na 3 TB.
      VPS umístěný v DC Brno nemá QoS a měsíční limit přenosů je stanoven na
      1 TB.
    - VPS je zálohován 1x denně, uchovává se 14 snapshotů zpětně.
  2. Playground virtuální server (pVPS) je OpenVZ kontejner, který si člen
     může sám vytvořit přes IS Spolku. Slouží zejména jako nástroj pro testování
     nové konfigurace, apod., pVPS není určený pro produkční nasazení.
    - Playground VPS má omezenou životnost na 1 měsíc, Rada může na žádost člena
      v oprávněných případech životnost pVPS prodloužit.
    - pVPS je parametry obdobný produkční VPS, s výjimkou CPU, pVPS má dostupná
      jen 3 jádra CPU; pVPS není zálohována.
  3. Network attached storage - NAS je úložiště, přes IS Spolku připojitelné do
     libovolných VPS člena.
    - Každý člen má v rámci základních prostředků dostupných 250 GB kapacity na
      NAS.
    - Prostor na NAS není zálohovaný.

2. Navyšování prostředků dostupných členovi
  1. Výši členských příspěvků v závislosti na navýšení prostředků člena upravuje
     Finanční řád.
  2. VPS je možné zvětšovat po celých násobcích velikosti základní VPS do
     maxima čtyřnásobku základních parametrů. V případě násobení velikosti se
     nezvyšuje počet IPv4 veřejných adres dostupných danému VPS. Počet
     dostupných CPU jáder se při násobení velikosti nezvyšuje, ale při případném
     limitování CPU prostředků je na znásobení VPS brán patřičný zřetel.
  3. VPS je možné navyšovat diskový prostor nezávisle na ostatních parametrech.
  4. Počet VPS je možné navyšovat, horní limit pro počet VPS není stanoven.
  5. NAS je možné zvětšovat po kroku 250 GB až do maximální velikosti 2 TB.

### Pravidla spravedlivého používání ("Fair Use Policy")

1. Člen je povinen používat dostupné prostředky Spolku tak, aby nenarušoval chod
   infrastruktury Spolku a využívání prostředků dalšími členy.
2. Rada spolku je oprávněna omezit CPU čas dostupný VPS i pVPS v následujících
   případech následovným způsobem:
   - v případě, že VPS využívá více jak 4 jádra po dobu delší, než 24 hodin, je
     Rada oprávněna snížit dané VPS dostupná CPU jádra na 4.
   - obdobné omezení má Rada možnost vztáhnout na VPS zatěžující více, než 4
     jádra v častých pravidelných intervalech.
   - pokud na VPS běží více jak 5 aktivních instancí herních serverů, má Rada
     právo toto VPS považovat za herní hosting.
   - Herním hostingům je snižováno dostupné CPU na polovinu jednoho jádra.
   - Primárním motivačním faktorem při limitování CPU je férové rozdělení
     výpočetní kapacity infrastruktury mezi všechny členy.
   - Zásadní výjimkou při tomto rozhodování jsou herní hostingy, které jako
     Spolek nechceme podporovat, nicméně samotné herní servery v rozumném
     množství na jednoho člena, jako herní hosting považovány nebudou.
   - Pokud člen nereaguje na notifikaci při snížení dostupných prostředků
     a nadměrné využívání stále trvá, má Rada právo snížit dostupná CPU jádra na
     dvě.

2. Základní pravidla při manipulaci se svěřenými prostředky
-----------------------------------------------------------

1. Člen využívá prostředky Spolku k libovolným účelům, pokud je využití v
souladu s platnými právními předpisy ČR a pokud využíváním nenarušuje provoz
ostatním členům.

2. Člen na infrastruktuře Spolku nesmí provozovat služby, které jsou primárně
určené ke škodění ostatním v rámci Internetu. Zrovnatak by člen měl co nejlépe
dbát na zabezpečení jeho prostředků proti neoprávněnému zneužití třetími
stranami.

3. Člen je povinen řešit připomínky Rady ke způsobům, jakým infrastrukturu
využívá. Zejména je povinen přezkoumat nastavení a provést nápravu, pokud z jeho
IP adres odchází do Internetu SPAM, nebo provoz podobného nevyžádaného
charakteru.

3. Postupy proti členům narušujícím provoz
------------------------------------------

1. Rada spolku dbá na nerušený a spolehlivý provoz infrastruktury Spolku.

2. V případě, že se zjistí, že člen využívá prostředky nevhodným způsobem, který
narušuje provoz ostatním, postupuje Rada od nejmírnějšího postihu k přísnějším.
Při takovém postupu je každý incident posuzován individuálně a kontextu celé
situace; Rada by měla zohlednit snahu a ochotu člena situaci řešit jako
významnou polehčující okolnost.

3. Rada je oprávněna použít těchto prostředků při postupu proti členům
narušujícím provoz:
  1. Notifikace člena přes dostupné komunikační kanály.
  2. Omezení dostupných prostředků tak, aby dopad narušitele byl minimální
     vzhledem k ostatnímu provozu.
  3. Pozastavení přístupu k prostředkům Spolku.
  4. V opravdu krajních případech, kdy člen nevykazuje žádný zájem situaci
     řešit, nebo opakovaným způsobem narušuje provoz i přes doporučení, jak
     situaci vyřešit, je Rada oprávněna narušujícího člena vyloučit.

4. Člen má právo se proti rozhodnutím Rady odvolat ke Kontrolní komisi, nicméně
omezení, která Rada na člena případně uvalila, platí dále, pokud z postupu
Kontrolní komise nevyplyne jinak.

