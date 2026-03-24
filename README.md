A projekt a BBBike adataival dolgozik, amelyek megtalálhatóak: https://download.bbbike.org/osm/bbbike/Budapest/

Az adathalmaz felhasználásához szükséges, hogy az a felhasználó saját gépén meglegyen, mert az túl nagy, hogy feltöltsük a GitHub-ra.
Ezt végzi a "Lement.ipynb" program, ami beszerzi a megfelelő adatokat és készít belőlük egy használható fájlt.

A "Beolvas.ipynb" használja fel a generált fájlt, és ezen keresztül fog működni a végleges program is.
(Jelenleg a Beolvas csak kiírja az adathalmazból generált gráf csúcs- és élszámát, hogy egy elképzelést adjon a méretéről.)
