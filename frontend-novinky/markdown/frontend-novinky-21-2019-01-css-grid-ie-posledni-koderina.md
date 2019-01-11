# CSS Grid: Autoplacement v IE (a poslední kurzy Webové kodéřiny)

Vítám vás v prvním newsletteru roku 2019!

## Autoplacement gridu v Internet Exploreru

Pokud Vzhůru dolů čtete pravidelně, už víte, že CSS Grid je možné [použít v Internet Exploreru](https://www.vzhurudolu.cz/prirucka/css-grid-msie) daleko častěji než tomu dosud bylo.

Vděčíme za to nedávným změnám v Autoprefixeru, který se naučil generovat kód tak, abychom mohli používat i vlastnosti jako `grid-gap` (mezera mezi buňkami) nebo  `grid-template-areas` (pojmenované oblasti).

O čem jsem ale zatím nepsal, jsou nové možnosti automatického umísťování prvků v mřížce. To je totiž třetí nejdůležitější vlastnost Gridu. A Explorer, který stále používá kolem desetiny českých uživatelů, ji nativně neumí.

Autoplacement znamená automatické umístění prvků v mřížce, aniž by to bylo definováno v CSS. Vezměme, že chceme layout 2 × 2. HTML kód vypadá takto:

```html
<div class="container">
  <p class="box">Box</p>
  <p class="box">Box</p>
  <p class="box">Box</p>
  <p class="box">Box</p>
</div>
```

Díky automatickému umístění bude v moderních prohlížečích stačit definovat mřížku v CSS:

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: auto auto;
}
```

Prvky se nám pěkně rozmístí. To ale nebude fungovat v Internet Exploreru. 

*TODO img modern/ie…*

Pro něj nám ale Autoprefixer přidá pseudotřídy:

```css
.container > *:nth-child(1) {
  -ms-grid-row: 1;
  -ms-grid-column: 1;
}

.container > *:nth-child(2) {
  -ms-grid-row: 1;
  -ms-grid-column: 2;
}
```

…a tak dále.

Neřeší to všechno, ale pro mnoho užití CSS Gridu to bude výborná pomoc. A o silný důvod navíc použít [CSS Grid](https://www.vzhurudolu.cz/prirucka/css-grid).

## Poslední kurzy Webové kodéřiny

Tímto vás zvu na poslední dva termíny kurzu [Dnešní webová kodéřina](https://www.vzhurudolu.cz/kurzy/webova-koderina). V Praze proběhne už 5. února a úplně poslední termín organizujeme *TODO…*

„Kodéřinu“, jako školení novinek a best-practice kolem HTML a CSS, vedu pod různými názvy už asi 9 let, ale je čas posunout se více směrem k mé aktuální hlavní specializaci – rychlosti webů.

*TODO IMG…*

Obsah kurzu ale rozhodně devět let starý není. V aktuálním vydání se můžete těšit právě na CSS Grid, Flexbox, základy automatizace pomocí NPM skripů, Gulpu a Gruntu nebo přístupnost.

Kurz je myslím skvělý pro juniorní kodéry nebo backendové vývojáře, kteří si chtějí udržet přehled o aktuálním vývoji CSS a HTML.

<br>

<p class="text-center">
<a class="vd-button" href="https://www.vzhurudolu.cz/kurzy/webova-koderina">Více o kurzu</a>
</p>

Konec hlášení. Podívejme se teď spolu ještě na sedm odkazů, které stojí za přečtení.

## Novinky a články, které by vám neměly uniknout

1. CSS Tricks: [2018 Staff Favorites](https://css-tricks.com/2018-staff-favorites/)
2. Vzhůru dolů: [Breakpointy v responzivním designu: Detailně a do hloubky](https://www.vzhurudolu.cz/prirucka/breakpointy)
3. 24 Ways: [Dynamic Social Sharing Images](https://24ways.org/2018/dynamic-social-sharing-images/)
4. Vzhůru dolů: [HTTP/2: S nasazením na nic nečekejte](https://www.vzhurudolu.cz/prirucka/http-2)
5. Performance Calendar: [Getting started with web performance: 2019 beginner’s guide](https://calendar.perfplanet.com/2018/getting-started-with-web-performance-2019-beginners-guide/)
6. Podcast ze Vzhůru dolů: [Frontendové technologie roku 2018](https://www.vzhurudolu.cz/podcast/130-podcast-technologie-2018)
7. [Lipsurf: Control the browser with your voice.](https://www.lipsurf.com/)

A to je vše, milí čtenáři. Přeji vám fajn rok 2019!

Martin Michálek  
[vzhurudolu.cz/martin](http://vzhurudolu.cz/martin)