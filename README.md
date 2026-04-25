A projekt a BBBike adataival dolgozik, amelyek megtalálhatóak: https://download.bbbike.org/osm/bbbike/Budapest/

Az adathalmaz felhasználásához szükséges, hogy az a felhasználó saját gépén meglegyen, mert az túl nagy, hogy feltöltsük a GitHub-ra.
Ezt végzi a "Lement.ipynb" program, ami beszerzi a megfelelő adatokat és készít belőlük egy használható fájlt.

A "Beolvas.ipynb" használja fel a generált fájlt, és ezen keresztül fog működni a végleges program is.
(Jelenleg a Beolvas csak kiírja az adathalmazból generált gráf csúcs- és élszámát, hogy egy elképzelést adjon a méretéről.)

A "Main.ipynb"-ben lesz az algoritmus törzse. Jelenleg még csak egyetlen függvény van benne, ami egy input helynévnek megkeresi a koordinátáit. Amennyiben az adott név már el van mentve a "place_coords.json" fájlba, onnan veszi elő, ha nincs, akkor az interneten keresztül keresi meg őket, és berakja a már meglévők közé.

A "place_coords.json" tartalmazza az általam, próbafuttatások során már elmentett helynév-koordinátapár adattömböket (ez per pillanat valószínűleg igen kevés).

##########################################################

A cél egy olyan program elkészítése, amely egy "mini google maps"-ként működik, azaz két inputként megkapott helyszín között képes megkeresni a legrövidebb utat.

Amennyiben ez a feladat túl egyszerűnek bizonyul, egy értelmes továbbfejlesztés volna az útkeresést több különböző algoritmuson keresztül is megvalósítani, és összehasonlítani azok futási idejét. Vagy emellett egy előfeldolgozási algoritmust készíteni, ami meggyorsítja a nagyméretű gráfban való útkeresést.
