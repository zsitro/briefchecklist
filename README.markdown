#BRIEF
##PROJEKT ALAPADATOK
### HASZNÁLHATÓSÁG
A wireframe, grafikai munkák megkezdése előtt célszerű ismerni a célközönség összetételét, leírása történhet az alábbi paraméterekkel:

* Férfiak/Nők,
* 18-25 éves korosztály
* egyetemisták/nyugdíjasok,
* bárki/vegyes/meghatározhatatlan `(marketing fail?)`

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
##### Felhasználók
* LÁTOGATÓ,
* REGISZTRÁLT LÁTOGATÓ,
* SUPERADMIN,
* ADMIN,

##### Fogalmak
* TERMÉK,
* KAMPÁNY,
* KOMMENT,

##### Műveletek
* REGISZTRÁCIÓ,
* RENDELÉS,
* KOMMENTELÉS

##### Oldal alkotóelemei
* FEJLÉC
	* FŐMENÜ
 	* ALMENÜ
  	* KERESŐDOBOZ
* (BAL)OLDALSÁV
	* BEJELENTKEZŐ DOBOZ
 	* KATEGÓRIALISTA
	* BANNER1
* TARTALOM
	* TERMÉKLEÍRÁS
 	* TERMÉKKÉP
  	* HASONLÓTERMÉKEK LISTA
* LÁBLÉC
	* LÁBLÉCMENÜ
 	* KERESŐDOBOZ
  	* LINKEK: FELHASZNÁLÁSI FELTÉTELEK,RÓLUNK, stb.

A leírásban pedig ezekkel a megnevezéssel legyenek hivatkozva egymásra.

####Példa
A __CATEGORYLIST__ oldalon egy kategórianévre kattintva a __FELHASZNÁLÓ__ átkerül a __PRODUCTLIST__ oldalra, ahol a kategóriában megtalálható publikált __TERMÉK__ek listáját találja. 

### ALOLDALAK
Aloldal lehet például __PRODUCTPAGE__,__CONTACT__,__ABOUT__, stb.

* Aloldalak felsorolása
	* Aloldal neve,
	* Mit lát a felhasználó az adott oldalon? (pl.: __TERMÉK__, __TERMÉK__-hez tartozó __KOMMENT__-ek)
	* Milyen műveleteket végezhet a __LÁTOGATÓ__/__REGISZTRÁLT LÁTOGATÓ__ az adott aloldalon? (pl.: __RENDELÉS__)
	* Aloldal fő funkciója/tartalma,

### BEVITELI MEZŐK
Ahol a projektben adatrögzítésre (pl.: REGISZTRÁCIÓ, KAPCSOLATOLDAL, KÉRDŐÍVOLDAL) van lehetőség, definiálni kell a LÁTOGATÓ-tól bekérendő adatok listáját és azokhoz tartozó attribútumokat.

#### Példa KAPCSOLATOLDAL-ra

* NÉV MEZŐ -> egysoros szöveg, kötelező
* NEME -> rádiógomb, kötelező, opciók: Férfi/Nő
* KÉRDÉS TÉMÁJA -> többszörös választás, nem kötelező, opciók: Technikai/Személyes/Árajánlat/Érdeklődés/Megrendelés/Hibabejelentés
* KÉRDÉS -> többsoros szöveg, maximum 1000 karakter, kötelező
* PRIORITÁS -> legördülő lista, kötelező, opciók: Sürgős/Válasz 2 napon belül/Válasz egy héten belül

### JOGOSULTSÁGOK
Ha a projekt típusa megköveteli, hogy a szoftver különböző módon kezelje a felhasználókat (lsd.: __LÁTOGATÓ__, __ADMIN__, stb.), akkor definiálni kell azok jogosultságait. 

Ezek lehetnek például:

#### Admin felületen:

* Olvasás,
* Módosítás,
* Törlés,

#### Publikus felületen:

Projekttől függően jellemzően __LÁTOGATÓ__t/__REGISZTRÁLT LÁTOGATÓ__t különböztetünk meg. Így lehet hozzájuk rendelni például:

* __LÁTOGATÓ__ hozzáférhet: 
	* LANDINGPAGE,
 	* MAINPAGE
* __REGISZTRÁLT LÁTOGATÓ__ hozzáférhet: 
	* LANDINGPAGE,
	* MAINPAGE,
	* CATEGORYLIST,
	* PRODUCTLIST, 
	* PRODUCTPAGE

##FUTTATÁSI KÖRNYEZET
###Hardver/Operációs rendszer

* Desktop-Laptop/Mobil-Tablet
* Windows/Linux/OSX

###Böngészők
####Modern böngészőkre tervezünk

* Internet Explorer 7+
* Mozilla Firefox
* Google Chrome
* Opera / Opera Mobile
* Safari

####Emellett igény esetén külön kérni kell

* Működés biztosítása IE6-ban is
* Mobil böngészőre tervezett/optimalizált design `(Részletezve talán máshol)`

##ERŐFORRÁSOK

* Mekkora látogatottságra számítanak?
	* Lesz e pontszerű (TV spot, Radio Ad, stb) kampánya az oldalnak?
	* Lesz e hosszú távú (pl.: Banner, plakát) kampánya az oldalnak?