# CSS Grid: Autoplacement v IE (a poslední kurzy Webové kodéřiny)

Vítám vás v prvním newsletteru roku 2019!

## Autoplacement gridu v Internet Exploreru

Pokud Vzhůru dolů čtete pravidelně, už víte, že CSS Grid je možné v řadě případů [použít i v Internet Exploreru](https://www.vzhurudolu.cz/prirucka/css-grid-msie).

Vděčíme za to nedávným změnám v Autoprefixeru, který se naučil generovat kód tak, abychom mohli používat i vlastnosti jako `grid-gap` (mezera mezi buňkami) nebo  `grid-template-areas` (pojmenované oblasti).

O čem jsem ale zatím nepsal, jsou nové možnosti automatického umísťování prvků v mřížce. Autoplacement je další důležitá vlastnost Gridu. A Explorer, který stále používá kolem desetiny českých uživatelů, ji nativně neumí.

Vezměme příklad: Chceme layout 2 × 2. HTML kód vypadá takto:

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

Prvky se nám pěkně rozmístí. Jenže smůla, tohle nebude fungovat v Internet Exploreru.

![Autoplacement v MSIE nefunguje](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/72631c1a-dd36-4104-8dde-3efbeed4c309.jpg)

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

Neřeší to všechno, ale máme tady o jeden silný důvod navíc použít [CSS Grid](https://www.vzhurudolu.cz/prirucka/css-grid).

Téma budu dále rozebírat na blogu, takže jej sledujte. Prakticky vyzkoušet jej můžete na jednom z mých kurzů. Teď trochu o něm.

## Poslední termíny kurzu kodéřiny

Tímto vás zvu na poslední dva termíny kurzu [Dnešní webová kodéřina](https://www.vzhurudolu.cz/kurzy/webova-koderina). V Praze proběhne už 5. února a úplně poslední termín organizujeme *TODO…*

„Kodéřinu“ vedu, jako školení novinek a best-practice kolem HTML a CSS, pod různými názvy už asi 9 let, takže budu muset zamáčknout slzu. Ale je čas posunout se více směrem k mé aktuální hlavní specializaci – rychlosti webů.

[![Poslední termíny školení kodéřiny](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/5109458a-06ac-469f-9a66-b4750c303511.jpeg)](https://www.vzhurudolu.cz/kurzy/webova-koderina)

Obsah kurzu ale rozhodně devět let starý není. V aktuálním vydání se můžete těšit právě na CSS Grid, Flexbox, základy automatizace pomocí NPM skripů, Gulpu a Gruntu. Také na tipy k přístupnosti, CSS vlastnostem, SVG a tak dále.

Kurz je myslím skvělý pro juniornější kodéry nebo backendové vývojáře, kteří si chtějí udržet přehled o aktuálním vývoji CSS a HTML.

<br>

<p class="text-center" markdown="1">
<a class="vd-button" href="https://www.vzhurudolu.cz/kurzy/webova-koderina">Více o kurzu</a>

<br><br>

<a class="vd-button" href="https://www.vzhurudolu.cz/blog/131-skoleni-6-duvodu">Proč jít na školení ze Vzhůru dolů</a>

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

A to je vše, milé čtenářky a milí čtenáři. Přeji vám fajn rok 2019!

Martin Michálek  
[vzhurudolu.cz/martin](http://vzhurudolu.cz/martin)