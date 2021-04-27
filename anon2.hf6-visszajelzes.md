**5a.** *10 pont*

**5b.** *10 pont*

**6.** *10 pont*

**7.** *7 pont*

"Ehhez a körhöz G-ben még páros körök vagy fák kapcsolódhatnak":

A páros körök és a fák nem egészen fedik le az összes esetet.
A páratlan körre kapcsolódhat mondjuk egy általános 2-színezhető gráf is (páratlan kör már biztos nem lesz a kapcsolódó gráf belsejében, de páros akárhány, akárhol)
Ennek a tárgyalása bonyolultabb, mint a páros kör esete, és nem illeszthető rá a BFS-fás bizonyítás sem.
Ha csak egy pontban kapcsolódik ez a gráf a páratlan körhöz, a kapcsolódási pont színe és a kapcsolódó gráf 2-színezhetőségéből kiindulva ki tudjuk színezni őket megfelelő módon, ez az egyszerűbb eset.
Ha viszont ez az általános 2-színezhető gráf 2 vagy több pontban kapcsolódik, akkor valamelyik két kapcsolódási pont között valóban lesz egy (más lehetőség híján) páros kör, viszont arra még "rá van nőve" tetszőlegesen kusza módon csomó minden, ami bonyolítja a tárgyalást.
Ekkor alkalmazható egy hasonló gondolatmenet: 

Két kapcsolódási pont között lesz egy út a kapcsolódó gráfban (n hosszú), és két út a körön (mondjuk k hosszú, páros ív, és l hosszú, páratlan ív, amik együtt ugye kiadják a páratlan kört).
Ekkor viszont az ezekből összerakott n+k, n+l hosszú körök valamelyike páratlan, és a  központi páratlan körtől különböző, ellentmondás.
Tehát kijött, hogy végülis a páratlan körre kapcsolódó gráfok mégiscsak egyetlen pontban kapcsolódhatnak, de ennek a miértjét le kell írni.

Összességében nagyon szép és igényes munka! Az utolsó feladatban elég rafinált módon "elbújt" egy eset, ami nem lett letárgyalva, és a tárgyalása nem triviális.
