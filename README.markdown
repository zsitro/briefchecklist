#BRIEF
##PLANNING


##WIREFRAME
###MEGNEVEZÉSEK:
A brief megírásakor a projektben szereplő (al)oldalak kapjanak egy-egy nagybetűs - a funkciójára, vagy tartalmára jellemző - nevet.
####Példák

* LANDINGPAGE,
* MAINPAGE,
* CONTACT,
* ABOUT,
* LOGINPAGE,
* CATEGORYLIST,
* PRODUCTLIST,
* PRODUCTPAGE,
* NEWSLETTER

Hasonló elvet követve a projekt többi alkotóelemeit is érdemes definiálni, amennyiben említésre kerülnek a dokumentációban:

####Példák
* LÁTOGATÓ,
* REGISZTRÁLT LÁTOGATÓ,
* SUPERADMIN,
* ADMIN,
* TERMÉK,
* KAMPÁNY,
* RENDELÉS

A leírásban pedig ezekkel a megnevezéssel legyenek hivatkozva egymásra.

####Példa
A __CATEGORYLIST__ oldalon egy kategórianévre kattintva a __FELHASZNÁLÓ__ átkerül a __PRODUCTLIST__ oldalra, ahol a kategóriában megtalálható publikált __TERMÉK__ek listáját találja. 

###

### Aloldalak
* Aloldalak felsorolása
** Aloldal neve
** Aloldal fő funkciója/tartalma

### Minden (al)oldalra
* Mit lát a felhasználó az adott oldalon?
	*
*

### JOGOSULTSÁGOK
Ha a projekt típusa megköveteli, hogy a szoftver különböző módon kezelje a felhasználókat (lsd.: LÁTOGATÓ, ADMIN, stb.), akkor definiálni kell azok jogosultságait. 

Ezek lehetnek például:

#### Admin felületen:

* Olvasás,
* Módosítás,
* Törlés,

#### Publikus felületen:

Projekttől függően jellemzően __LÁTOGATÓ__t/__REGISZTRÁLT LÁTOGATÓ__t különböztetünk meg. Így lehet hozzájuk rendelni például:

* __LÁTOGATÓ__ hozzáférhet: LANDINGPAGE, MAINPAGE, CATEGORYLIST, PRODUCTLIST
* __REGISZTRÁLT LÁTOGATÓ__ hozzáférhet: LANDINGPAGE, MAINPAGE, CATEGORYLIST, PRODUCTLIST, PRODUCTPAGE

* 
##FUTTATÁSI KÖRNYEZET
###Hardver/Operációs rendszer
*Desktop-Laptop/Mobil-Tablet
*Windows/Linux/OSX

###Böngészők
* Modern böngészők
* Működés biztosítása IE6-ban is?

##ERŐFORRÁSOK
* Mekkora látogatottságra számítanak?
	* Lesz e pontszerű (TV spot, Radio Ad, stb) kampánya az oldalnak?
	* Lesz e hosszú távú (pl.: Banner, plakát) kampánya az oldalnak?