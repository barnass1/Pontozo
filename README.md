# Pontozólap

Medve Barnabás

EM9NYU

Projekt rövid leírása:
Egy feladatok rögzítésére szolgáló winforms, illetve egy webalkalmazás. Indulásnál a formsba egy datagridview-ba tölti a feladatokat, illetve mellé egy listbox-ba a felhasználókat. A formsban új felhasználókat és feladatokat lehet hozzááadni, illetve a feladatokat szerkeszteni is lehet. A webapp-ban az index.html-be betölti a feladatokat, a felhasználókat mellé írja, ezeket törölni lehet, illetve új feladatokat is lehet hozzáadni.


# Hozott anyagok:
## Adatbázis
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2019.00.30.png)
- 2x1p Az alkalmazásban használt táblánként pont (Tasks, Users)
- 2p Az adatbázis saját Azure SQL szerveren van
- 1p Az adatbázis adatainak forrásmegjelölése értsd: miből készült és hogyan:

Az adatbázis egy SQL query-vel készült, adatait a Users táblában tárolt felhasználó adja hozzá a Tasks táblához.

## Weboldal
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2020.26.51.png)
- 1x1p A weboldalnak van egy értelmezhető struktúrája
- 1x1p A weboldal dinamikus tartalommal tölthető fel adatbázison keresztül
- 1x1p A weboldal használ legalább 20 sor értelmes css-t
- 1x1p A weboldal javascriptet használ API végpont által szolgáltatott adatok betöltésére, hozott anyagként
- 1x1p A weboldal javascriptje más funkciót is ellát, mint az adatok betöltése

## Egyéb, extra
- 2x1p Scaffold-DbContext használata (ajándék)

# Windows Forms Application
## User Interface
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2020.21.25.png)
- 1x2p Az alkalmazásból a kilépés csak megerősítő kérdés után lehetséges.
- 2x1p Többablakos alkalmazás legalább két felugró ablakkal. Minden Form-nak saját osztályon kell alapulnia, és funcionalitással kell rendelkeznie. Az ablakok nyílhatnak gombokkal vagy felső menüből is.
- 1x2p Anchorok alkalmazása: az alkalmazás egészében meg van oldva, hogy az ablak átméretezésekor ki legyen használva a rendelkezésre álló terület.

## Tábla adatainak megjelenítése ListBox-ban.
- 1x2p Adatok megjelenítése
- 1x2p Ha az adatok tetszőleges módszerrel, pl. TextBox-on keresztül szűrhetőek.

## Tábla adatainak megjelenítése DataGridView-ban
- 1x2p Adatok megjelenítése
- 1x2p Ha a tábla idegen kulcsot is tartalmaz, melynek megjelenítése DataGridViewComboBoxColumn-on keresztül történik.

## Adatkötés BindingSource -on keresztül
- 1x2p Működő BindingSource

## Új rekord rögzítése
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2020.25.37.png)
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2020.25.29.png)
- 1x2p Ha csak az idegen kulcsok vannak felvéve
- 1x1p Ha legalább egy nem kulcs mező, pl. Mennyiség is fel van véve
- 1x2p Ellenőrzéshez kötött adatfelvitel (egyszerű validáció pl: String.IsNullOrEmpty())
- 1x2p Felugró ablakon keresztül történik Ok és Mégse gombbal
- 1x2p Ha az űrlap legördülő dobozon vagy listán keresztül beállítható idegen kulcsot is tartalmaz
- 2x1p A kitöltési hiba ErrorProvider-en keresztül kerülnek köközlésre a felhasználóval, hibás kitöltés esetén nem enged rányomni az Ok gombra
- 1x2p Regex alapú validáció
- 1x1p Hibás kitöltés esetén nem lehet megynomni az Ok gombot.
  
## Rekord törlése
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2020.25.44.png)
- 1x2p Sikeres törlés
- 1x2p Megerősítéshez kötött törlés

# ASP .NET
## ASP .NET alkalmazás, melyet lehet a Forms alapú projekttel közös solution-ben létrehozni.
- 1x2p program.cs beállítása wwwroot mappában tárolt statikus tartalmak megosztására
  
## API végpontok
![](https://github.com/barnass1/Pontozo/blob/main/Kepek/Screenshot%202024-12-14%20at%2020.26.41.png)
- 1x3p Teljes SQL tábla adatainak szolgáltatása API végponton keresztül
- 1x2p SQL tábla egy választható rekordjának szolgáltatása API végponton keresztül
- 1x3p SQL tábla egy választható rekordjának törlése
- 1x5p Új rekord felvétele HttpPost metóduson keresztül SQL táblába

# Pontszám: 
