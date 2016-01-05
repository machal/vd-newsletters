# Rok 2015 ve webdesignu. S důrazem na kodéřinu pochopitelně

## 1) Javascriptový boom - React, isomorfní appky a spol.

Pro invazi JS ekosystému loni dorazilo mnoho nových posil. Pobláznění Reactem je jen jeden z projevů nevyhnutelného nástupu Javascriptu na trůn. Ovšem jen u webových aplikací, protože…

##  2) Weby a webové aplikace jsou si ještě vzdálenější

React, Browserify, Webpack, CssModules… tohle všechno je skvělé. Pro webové aplikace. Pokud ale vyrábíte vyhledávačem indexovatelné statické weby, novinky javascriptového ekosystému až tak neoceníte. Potřebujete Javascript na serveru nebo totální závislost na frontendovém JS. Obojí je pro existující obsahové weby těžce zchůdné. Do budoucna je možné čekat, že současné webařské technologické ekosystémy (PHP, Rails…) převezmou leccos z aktuálního vývoje kolem Javascriptu. A ti co mohou, půjdou i u obsahových webů do izomorfního přístupu – JS na frontendu i backendu. Do té doby vězte, že za jQuery se u statických webů stydět nemusíte. Nástroje pro tvorbu webů a webových aplikací si nikdy nebyly dál a to jsme ještě neskončili.

## 3) Adobe Comet

Naprosto pochopitelný úkrok od Photoshopu jako nástroje pro webdesign pokračuje. Blížíme se do cílové rovinky? Po přechodu velké části designérů na Sketch, po ukončení vývoje Fireworks, po letech čtení Photoshop hejtů… Po tom všem loni Adobe přišlo s demem nástroje pro komplexní návrh UX. Zatím ho nelze hodnotit, ale [vypadá skvěle](http://landing.adobe.com/en/na/products/creative-cloud/comet/229818-notifyme.html) a hlavně nám ukazuje, že od Photoshopu nás chce osvobodit i jeho mateřská firma. Doufejme, že to nebude jen kometa.

## 4) EU cookies

Už máte cookie lištu? Když používáte běžné Google Analytics, žádnou ani nepotřebujete. Tohle téma se intenzivně řešilo, ale jen málokdo o něm měl dost informací. [Ty najdete v článku.](http://www.vzhurudolu.cz/blog/36-eu-cookies)

## 5) PostCSS

Postprocessing CSS preprocesory zatím nezabije. Jen jim bude postupně ubírat pole působnosti. Ukazuje se, že některé úkoly je lepší svěřit právě následnému zpracování – třeba doplňování `px` fallbacků pro `rem` nebo automatické vkládání prefixů. [Více v článku.](http://www.vzhurudolu.cz/blog/34-css-postprocessing)

## 6) AMP, Progressive Web Apps a další novinky mobilního webu

… a taky Mobilegeddon, Service Worker, Physical Web nebo `navigator.connection`… kolem mobilních webů se toho loni dělo hodně! Více [v čerstvém článku na Vzhůru dolů](http://www.vzhurudolu.cz/blog/45-2015-mobilni-web).

## A co další? Tyhle nejsou nové, ale výrazně se prosadily do mainstreamu

- **Google Material Design** – všímáte si, jak dnešní korporace soupeří designovými systémy? Podívejte se na mobilní aplikace co nejčastěji používáte a asi budete souhlasit, že 2015 byl rokem materiálního designu od Google.
- **srcset/sizes a picture** – shoda mezi výrobci prohlížečů a vysoká míra užitečnosti pro uživatele. Jak řešit responzivní obrázky? [Takto.](http://www.vzhurudolu.cz/prirucka/responzivni-obrazky) 
- **Responzivní design** – zkušenějším to bude znít neuvěřitelně, ale teprve [od srpnového Mobilegeddonu](http://blog.bloxxter.cz/stitky/mobilegeddon/)  přestávám potkávat lidi tvrdící, že připravovat weby pro mobily není potřeba.
- **SVG** – vektorovou grafiku potřebujeme nejen kvůli „Retina displejům“. SVG přináší i dlouhou řadu inovací do návrhu a implementace uživatelských rozhraní. Ještě o něm hodně uslyšíme.
- **Flexbox** – ještě neděláte layouty komponent s jeho pomocí? Přišel čas [koupit ebook](http://www.vzhurudolu.cz/ebook). 
- **Style Guides** – aka „vlastní Bootstrapy“. Na jejich skutečně masivní rozšíření si počkáme, ale loni si našly cestu i do mnoha českých firem. 

## Rychlé tipy a triky

- **[Interaktivní výuka CSS vlastnosti flexbox.](http://flexboxfroggy.com/)** Flexbox Froggy je super nápad, jak pochopit možnosti flexboxu pomocí chytlavé hry. Pěkný počin.
- **[Why I'm Excited About Native CSS Variables](http://philipwalton.com/articles/why-im-excited-about-native-css-variables/)** CSS proměnné se liší od těch, které známe z preprocesorů. Článek popisuje nové techniky návrhu stylů, které se nám díky nim otevírají.
- **[Přehled kurzorů.](http://css-cursor.techstream.org/)** Upravit vzhled kurzoru se může hodit např. pokud pracujete na vývoji webových aplikací. Tento web vše přehledně shrnuje a přidává informaci o podporovaných prohlížečích.
- **[CSS Modules - Welcome to the future.](http://glenmaddern.com/articles/css-modules)** Při psaní stylů pro webové aplikace musíme neustále myslet na správnou volbu názvů tříd - snažíme se je dělat co nejobecnější. S CSS moduly tento problém odpadá. Už nikdy nebudete muset myslet na to, zda omylem nepřepíšete styly někde jinde.
- **[TIP: přiblížení produktové fotografie bez Javasscriptu](https://medium.com/@mjtweaver/css-product-magnification-without-javascript-497ab5932419#.2ktu9wese)** - Tento trik se často používá u eshopů. Existuje řada javascriptových pluginů. Toto elegantní řešení však ukazuje, že si můžeme vystačit jen s CSS.
- **[VIDEO 1: Lets move!](https://www.youtube.com/watch?v=J6wUmQDQBkw)** - Zajímavá přednáška ukazující hned několik triků, se kterými lze vylepšit animace na webu. Například zjistíte, že pro animování se nevyplácí používat jednoduché funkce jako `linear` či `ease-in`, protože nevytváří dojem přirozeného pohybu.
- **[VIDEO 2: Troubleshooting rendering performance issues](https://www.youtube.com/watch?v=2vFrZXWiwIc)** - Užitečné video z dílny Harry Robertse skvěle popisuje možnosti Chrome DevTools při odkrývání problémů ve vykreslování webu. Zapněte si „Enable Paint Flashing” a sledujte co se překresluje např. během scrollování.

## Nové školení: SVG

_TODO IMG_

SVG má ohromný potenciál a na tomhle školení se ho naučíte pořádně do hloubky. Školení vede Michal Matuška, senior vývojář u SuperKodérů.  Opět v pražském KC Greenpoint.

<p class="text-center">
<a href="/kurzy/svg#objednavka" class="button">Objednat místo na SVG školení</a>
</p>

A pozor, nové termíny všech kurzů [začínají už koncem ledna](http://www.vzhurudolu.cz/kurzy).

Do Nového roku přejeme hodně sil a spoustu příjemných projektů.

Martin Michálek ([@machal](http://www.twitter.com/machal)) & Martin Pešout ([@martinpesout](http://www.twitter.com/martinpesout))

PS: Máme také newsletter k pořádaným školením. Může se hodit – jako první se například dozvíte o nových školeních. [Přihlaste se zde](http://eepurl.com/SbG71).
