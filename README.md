A projekt a BBBike adataival dolgozik, amelyek megtalálhatóak: https://download.bbbike.org/osm/bbbike/Budapest/

Az adathalmaz felhasználásához szükséges, hogy az a felhasználó saját gépén meglegyen, mert az túl nagy, hogy feltöltsük a GitHub-ra.
Ezt végzi a "Lement.ipynb" program, ami beszerzi a megfelelő adatokat és készít belőlük egy használható fájlt.

A "Beolvas.ipynb" illusztrálja milyen módon történik a fájl beolvasása és ad egy képet a felhasznált adathalmaz méretéről.

A "place_coords.json" tartalmazza az általam, próbafuttatások során már elmentett helynév-koordinátapár adattömböket (ez per pillanat valószínűleg igen kevés).

A "Main.ipynb"-ben van az algoritmus törzse. Jelenleg a következő funkciókat tartalmazza:
- Képes elkészíteni, menedzselni és felhasználni a "place_coords.json" könyvtárat, hogy gyorsítsa a helymeghatározást.
- Megtalálni a felhasználó által keresett kiinduló- és célpontokat.
- A find_route függvényen keresztül megkeresni a legrövidebb utat a két pont között.
- A compress_route függvényen keresztül ezt olvasható navigációs instrukciókká alakítani.

##########################################################

A projektben felhasznált könyvtárak, modulok és package-ek:
- osmnx: a földrajzi adatok kezelésére és a gráfmodellhez
- rapidfuzz: a szövegkereséshez
- json: a felhasználó által már keresett helyszínek mentésére
- math, heapq: az algoritmusok megvalósítására

##########################################################

A cél egy olyan program elkészítése, amely egy "mini google maps"-ként működik, azaz két inputként megkapott helyszín között képes megkeresni a legrövidebb utat.

Amennyiben ez a feladat túl egyszerűnek bizonyul, egy értelmes továbbfejlesztés volna az útkeresést több különböző algoritmuson keresztül is megvalósítani, és összehasonlítani azok futási idejét. Vagy emellett egy előfeldolgozási algoritmust készíteni, ami meggyorsítja a nagyméretű gráfban való útkeresést.
