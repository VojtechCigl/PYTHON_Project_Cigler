# PYTHON_Project_Cigler
Edinburgh-bikes-project


Zadání projektu:

V Edinburghu, stejně jako v dalších městech, funguje systém "bike sharing" - ve městě jsou stanice s koly, člověk si může nějaké půjčit a potom ho vrátit v nějaké další stanici. Problém je, že v některých stanicích se kola pravidelně hromadí a jinde naopak chybí.

K dispozici jsou data o všech výpůjčkách (edinburgh_bikes.xlsx, edinburgh_weather.csv). Datový soubor obsahuje celkem 438259 záznamů o jízdách uskutečněných v období 15.9.2018 až 30.6.2021. Každý záznam obsahuje datum a čas výpůjčky a vrácení kola, dobu trvání výpůjčky v sekundách, identifikaci odjezdové a příjezdové stanice (číslo, název, popis, souřadnice).

Úkolem je zpracovat relevantní data a zjistit z nich následující informace:
  
1. Jak dlouho trvá jedna výpůjčka kola (jedna jízda)?
2. Jaké stanice jsou aktivní a neaktivní?
3. Na jakých stanicích se kola hromadí a kde jich je nedostatek?
4. Jaké jsou vzdálenosti mezi jednotlivými stanicemi?
5. Jak se vyvíjí poptávka po kolech v čase a jaké jsou příčiny výkyvu poptávky?
6. Jaký vliv má na poptávku počasí?
7. Půjčují si lidé kola více o víkendu, nebo v pracovních dnech?

Výsledek analýzy

1. Jak dlouho trvá jedna výpůjčka kola (jedna jízda)?
  - nejvíce výpůjček trvá 5-10 minut
  - polovina výpůjček trvá do 20 minut
  - 99.9 % výpůjček trvá do 6,5 hodiny

2. Jaké stanice jsou aktivní a neaktivní?
  - hranice pro neaktivní stanice byla stanovena na 1 odjezd a 1 příjezd týdně
  - rozsah aktivity stanic je 0-32 odjezdů/příjezdů za den
  - polovina stanic má aktivitu 2 odjezdy/příjezdy za den
  - počet neaktivních stanic je 42 (21 % celku)

3. Na jakých stanicích se kola hromadí a kde jich je nedostatek?
  - na 11 stanicích se kola hromadí (přírůstek > 1 kolo za den)
  - na 16 stanicích je nedostatek kol (úbytek > 1 kolo za den)
4. Jaké jsou vzdálenosti mezi jednotlivými stanicemi?
  - byla vytvořena interaktivní mapa rozmístění stanic
  - byla vypočítána matice vzdáleností 199x199 stanic viz výsledky analýzy
5. Jak se vyvíjí poptávka po kolech v čase a jaké jsou příčiny výkyvu poptávky?
  - poptávka je závislá na sezóně (vliv ročních období)
  - v roce 2020 došlo k nárůstu poptávky - možný vliv koronaviru (averze k hromadné dopravě)
6. Jaký vliv má na poptávku počasí?
  - poptávku ovlivňují mezní hodnoty teploty vzduchu (okolí bodu mrazu a 20 °C)
  - poptávka je výrazně ovlivněna deštěm a také vyššími hodnotami rychlosti větru
7. Půjčují si lidé kola více o víkendu, nebo v pracovních dnech?
  - o víkendu je vyšší zájem o kola oproti pracovním dnům
  - nárůst poptávky je patrný již v pátek

  



