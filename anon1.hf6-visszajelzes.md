**5a.** 
*0 pont a 10-ből*

Valójában minden csúcs fokszáma 10 lesz, mert a 20 halmazból (összes halmaz) kell levonni azokat, amikkel 3 közös eleme van a halmaznak (=önmaga, 1db), és amivel 2 közös elem van (3 alatt a 2 * 3 alatt az 1 = 9). Így Euler körséta és séta is lesz. Persze ehhez kell az összefüggőségről is mondani valamit.

**5b.**
*3 pont a 10-ből*

De nem lesz összefüggő, az is szükséges hozzá. Él nem futhat olyan A sorozat között, amiben páratlan sok egyes van, és olyan B között, amiben páros sok, tehát legalább két elkülönült komponens lesz. Vagyis nem lesz benne egyikfajta Euler-séta sem.

**6.**
*3 pont a 10-ből*

- a "2 = 3 ellentmondás" sorhoz:
Jó a gondolat, de az a baj, hogy 3 hosszú körre működik ilyen szépen, tetszőleges `2n+1` hosszúra még kell indoklás, ez nem elég. Kiegészíthető valahogy úgy a dolog, hogy ha egy szomszédos csúcsra lépünk, akkor 1 bit fog különbözni, ha még egyet lépünk, akkor vagy 0 vagy 2 bitben különbozhetünk a kiindulási csúcstól, ha még egyet akkor páratlan sokban, stb. Ha egy utat bejárva páratlan sokat lépünk, akkor páratlan bitben térhetünk el a kiindulási csúcstól, így ha lenne páratlan kör, akkor azon körbemenve visszaérünk az eredeti csúcsba, de az eredeti csúcs nem különbözhet páratlan sok bitben önmagától.
- egy lehetséges elegáns megoldás: válasszuk szét a csúcsokat két kategóriába: páros sok 1-et és páratlan sok 1-et tartalmazók. Egyazon kategoriába tartozó csúcsok között nem futhat él, mert egy bitet átállítva az 1-esek számának a paritása megváltozik, tehát az éllel összekötött élekben az 1-ek számának paritása szükségszerően különböző. Így a két kategóriát két színnel színezve valid színezést kapunk
- Az ötlet működik 3 hosszú körökre, és kiterjeszthető általánosan, de az nincs leírva, hogy hogyan. Hiányos indoklás, de helyes végkövetkeztetés

**7.**
*4 pont a 10-ből*

- első bekezdés, omegás rész: Így van, bár nem egészen tudom kivenni a megkötést omegára, de feltételezem hogy kisebb vagy egyenlő mint 3

- második bekezdés: Nem világos a fogalmazás, erre vigyázz zh-n. Csak egy sajátos esetet tárgyalsz, az általános ötlet, ha jól értettem, az az, hogy hogy veszed a páratlan kört `A_1`, `A_2`,...,`A_2n+1` alakban (csúcsok sorozata), és ha lenne egy `B` pont a körön kívűl, ami össze lenne kötve `A_i`-vel és `A_j`-vel, akkor a gráfban már több páratlan kör is lenne. De ezt meg kell indokolni, hogy miért! Jelen esetben azért, mert a két csúcs között a körön egyik körüljárási irányban páratlan, a másikban páros sok él van. Ha az előbbihez hozzáveszed a `BA_i` és `BA_j` éleket, akkor kapsz egy az elsőtől különböző páratlan kört, ellentmondás

- És amúgy mi történik, ha a fenti kiegészítésben a `B` nem közvetlenül kapcsolódik az `A_i` és `A_j`-hez, hanem mondjuk egy `k` és `l` hosszú úton keresztül, amely út élei és csúcsai nincsenek a körön? Erre is ki lehet terjeszteni az állítást, de ezt is tárgyalni kell!

- utolsó bekezdés: Nem egészen precíz itt a fogalmazás, de értem mire gondolsz. Ha kiveszed a páratlan kört, akkor a gráf szétesik 2-színezhető komponensekre, amik csak egy csúcsban kötődnek az eredeti körhöz, így pedig átgondolható hogy 3 szín miért elég. De az indoklás nagyon hiányos

- A gondolatmeneted kiegészítehtő egy teljes megoldássá, de önmagában nagyon hiányos. A precizitást gyakorold, mert vannak jó ötleteid, de a javítónak nem lesz energiája, hogy helyetted kiegészítse a megoldást
