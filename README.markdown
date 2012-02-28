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
 	* NYELVVÁLASZTÓ
 	* KERESŐDOBOZ
  	* LINKEK: FELHASZNÁLÁSI FELTÉTELEK,RÓLUNK, stb.

A leírásban pedig ezekkel a megnevezéssel legyenek hivatkozva egymásra.

>####Példa
>A __CATEGORYLIST__ oldalon egy kategórianévre kattintva a __FELHASZNÁLÓ__ átkerül a __PRODUCTLIST__ oldalra, ahol a kategóriában megtalálható publikált __TERMÉK__ek listáját találja. 

### ALOLDALAK
Aloldal lehet például __PRODUCTPAGE__,__CONTACT__,__ABOUT__, stb.

* Aloldalak felsorolása
	* Aloldal neve,
	* Mit lát a felhasználó az adott oldalon? (pl.: __TERMÉK__, __TERMÉK__-hez tartozó __KOMMENT__-ek)
	* Milyen műveleteket végezhet a __LÁTOGATÓ__/__REGISZTRÁLT LÁTOGATÓ__ az adott aloldalon? (pl.: __RENDELÉS__)
	* Aloldal fő funkciója/tartalma,

### BEVITELI MEZŐK/ŰRLAPOK
Ahol a projektben adatrögzítésre (pl.: REGISZTRÁCIÓ, KAPCSOLATOLDAL, KÉRDŐÍVOLDAL) van lehetőség, definiálni kell a LÁTOGATÓ-tól bekérendő adatok (BEVITELI MEZŐk) listáját és azokhoz tartozó attribútumokat.

#### Beviteli mezők típusai

* Egysoros szöveg
* Többsoros szöveg
* Fájl
* Jelszó
* Rádió gomb
* Jelölőnégyzet
* Legördülő lista
* Többértékes választó lista

[KÉP: Beviteli mezők típusai](https://github.com/zsitro/briefchecklist/blob/master/assets/hu-sample-form-elements.png?raw=true)


#### Beviteli mezőkhöz tartozó attribútumok
* Felirat
* Kötelező/Nem kötelező kitölteni
* Formátum
	* Szöveg 	
  	* Számok
   	* Alfanumerikus
   	* Egyszerűsített HTML (pl.: `<strong>`,`<i>`,`<a>`,`<h1>`,stb.) 
	* Validálás nélküli mező (csak ADMIN felületen elérhető)
	* E-mail cím
	* Egyedi
* Minimum-maximum hossz
* Minimum-maximum érték (szám esetén)
* Opcióválasztó mező esetén opciók listája
* Beírás után át kell e alakítani az adatot? (Pl.: 10000000 esetén -> 10.000.000)
* Ha a mező kitöltése kötelező -> kihagyás/rossz kitöltés esetén hibaüzenet szövege
* Szükség lesz e például admin felületen a bevitt mezőre szűrni/keresni

#### Űrlap (FORM) adatai
* Hibás adatok esetén az üzenet megjelenésének helye:
	* Az űrlap tetején/alján mind
 	* Az egyes mezők mellett egyenként
  	* Felugró ablakban mind


>#### Példa KAPCSOLATOLDAL-ra
>
>* NÉV MEZŐ -> egysoros szöveg, kötelező
>* NEME -> rádiógomb, kötelező, opciók: Férfi/Nő
>* KÉRDÉS TÉMÁJA -> többértékes választó lista, nem kötelező, opciók: Technikai/Személyes/Árajánlat/Érdeklődés/Megrendelés/Hibabejelentés
>* KÉRDÉS -> többsoros szöveg, maximum 1000 karakter, kötelező
>* PRIORITÁS -> legördülő lista, kötelező, opciók: Sürgős/Válasz 2 napon belül/Válasz egy héten belül

### JOGOSULTSÁGOK
Ha a projekt típusa megköveteli, hogy a szoftver különböző módon kezelje a felhasználókat (lsd.: __LÁTOGATÓ__, __ADMIN__, stb.), akkor definiálni kell azok jogosultságait. 

>Ezek lehetnek például:
>
>#### Admin felületen:
>
>* Olvasás,
>* Módosítás,
>* Törlés,
>
>#### Publikus felületen:
>
>Projekttől függően jellemzően __LÁTOGATÓ__t/__REGISZTRÁLT LÁTOGATÓ__t különböztetünk meg. Így lehet hozzájuk rendelni például:
>
>* __LÁTOGATÓ__ hozzáférhet: 
>	* LANDINGPAGE,
> 	* MAINPAGE
>* __REGISZTRÁLT LÁTOGATÓ__ hozzáférhet: 
>	* LANDINGPAGE,
>	* MAINPAGE,
>	* CATEGORYLIST,
>	* PRODUCTLIST, 
>	* PRODUCTPAGE

## l18n
A projekt publikus felületének nyelvét egy nyelv esetén is meg kell adni, ha több nyelvű oldalról van szó, akkor felsorolással kell megadni.

Ha igény van - akár egy vagy többnyelvű oldal esetén is - arra, hogy a megjelenő információk időzónáktól függően jelenjenek meg (pl.: egy rendezvény időpontja), akkor azt részletes leírásban kell közölni.


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

### Preferált/kért technológiák használata

####Platform or watever
* HTML
* Flash
* Java
* etc..

#### PHP Keretrendszerek

* Drupal
* Wordpress
* Zend/Yii/Symfony/etc

#### HTML
* HTML5
* XHTML Transitional
* XHTML Strict


###Erőforrások

* Mekkora látogatottságra számítanak?
	* Lesz e pontszerű (TV spot, Radio Ad, stb) kampánya az oldalnak?
	* Lesz e hosszú távú (pl.: Banner, plakát) kampánya az oldalnak?