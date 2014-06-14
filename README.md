Teremfoglalás kezelő
===============


Készítsünk programot, amely elősegíti termek foglalását az oktatók számára. A rendszer
háromféle termet tart nyilván, amelyek a következő adatokkal rendelkeznek:

• Előadó terem (0-s kód): terem neve, az ülőhelyek száma, van-e beépített projektor
(0: nincs, 1: van)
• Szeminárium terem (1-es kód): terem neve, az ülőhelyek száma, valamint a tábla
típusa (0: krétás, 1: filces).
• Gépterem (2-es kód): terem neve, az ülőhelyek száma, számítógépek száma.

Ezen felül minden teremre kiszámolható a kapacitása a következőeknek megfelelően:

• Előadó terem: ha van projektor, és azt igénybe veszik, akkor az ülőhelyek
számának 115%-a, mivel ekkor úgyse fognak bejönni a hallgatók órára, különben
a ülőhelyek száma.
• Szeminárium terem: ha filces a tábla, az ülőhelyek száma, ha krétás, akkor az
ülőhelyek száma -6 fő, mert az első sorba senki sem ül a szálló krétapor miatt.
• Gépterem: a számítógépek számának 90%-a (mert a többi biztos rossz) +10 fő
(akik úgyis laptoppal járnak), de maximálisan az ülőhelyek száma.

A program az adatokat szöveges fájlból olvassa be, amelynek minden sora egy terem
adatait tartalmazza a megadott sorrendben. Legyen lehetőség a felhasználónak megadni,
mekkora kapacitású termet akar foglalni, géptermet szeretne-e, legyen-e projektor
(gépteremben mindig van, szeminárium teremben nincs), illetve filces táblát szeretne-e
(gépteremben mindig filces a tábla, előadóban sosem), és a program ekkor listázza ki
azokat a termeket, amelyek az igénynek eleget tesznek, vagy írja ki, hogy nincs a
keresésnek megfelelő terem.
