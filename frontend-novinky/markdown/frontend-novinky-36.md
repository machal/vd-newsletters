# Nová CSS vlastnost content-visibility a říjnová školení

Milé čtenářky, milí čtenáři,

vítám vás zpět z prázdnin a doufám, že jste si je užili!

Dnes jsem pro vás připravil tip na zajímavou novou CSS vlastnost, dále vám chci říct, že se těším, že se snad konečně uvidíme u říjnových kurzů, no a na konec jsem si nechal tradiční tipy na čtivo nebo poslech novinek ze světa CSS a JS.

## Vlastnost content-visibility – „lazy loading“ pro rendering

Představte si, že máte komplexní layout a víte, že velká část z něj zůstane uživatelům minimálně zpočátku vykreslování skrytá, protože není vidět v prvním viditelném viewportu.

![content-visbility](https://mcusercontent.com/d6be2f1899eba6a7651157403/images/85e8ca90-8ba2-4c8c-ab55-ba2dd383da0e.jpeg)

Docela by se hodilo, aby prohlížeč při výpočtu vzhledu stránky vynechal část, kterou uživatel nevidí. Přesně pro tyhle účely se hodí deklarace `content-visibility:auto`, kterou teď začal podporovat Chrome.

Vlastnost může ušetřit desítky až stovky milisekund při počítání vykreslování stránky. [Una Kravets](https://web.dev/content-visibility/) udělala demo, kde je vidět sedmkrát méně času, spotřebovaného při renderingu. [Jan Šablatura](https://www.zdrojak.cz/clanky/content-visibility-jedna-css-vlastnost-vsem-rychle-vykresleni-kaze/) to vyzkoušel na webu českých Novinek a teoreticky by tam prý došlo k ušetření více než 40 % renderovacího času.

Vlastnost vypadá skvěle, ale ještě si počkejte na můj článek. Po testech si totiž nemyslím, že bychom ji měli bezhlavě aplikovat všude a očekávat zázraky. Text vyjde tento týden na Vzhůru dolů.

## Rikiho a Michalovy webináře

V těchto dnech běží vaše poslední šance dostat se na Rikiho webináře o javascriptových nástrojích:

* [NPM a Yarn](https://www.vzhurudolu.cz/kurzy/webinar-npm-yarn) — st 9. 9.
* [Principy Webpacku](https://www.vzhurudolu.cz/kurzy/webinar-webpack) — st 16. 9.
* [Praktický úvod do Vue](https://www.vzhurudolu.cz/kurzy/webinar-vue-uvod) —  čt 17. 9.

Michal Matuška už také intenzivně pracuje na přípravě svých webinářových lekcí:

* [Rychlost v Chrome DevTools](https://www.vzhurudolu.cz/kurzy/webinar-devtools-rychlost) — út 22. 9.
* [Animace s knihovnou GSAP](https://www.vzhurudolu.cz/kurzy/webinar-gsap) — st 23. 9.
* [Variabilní fonty](https://www.vzhurudolu.cz/kurzy/webinar-variabilni-fonty) — út 29. 9.
* [Optimalizace SVG](https://www.vzhurudolu.cz/kurzy/webinar-svg-optimalizace) — st 30. 9.

Všechny začínají v 17:00, trvají zhruba hodinu (podle množství dotazů), budou vysílány přes platformu Zoom a pokud termín nestíháte, objednejte si je i tak. Dostanete totiž týdenní přístup k záznamu.

## Prezenční školení v Praze a Brně

Vy, kteří na naše školení chodíte, už víte co vás čeká – celý jeden den, zkušený lektor, jedno téma do hloubky.

Můžete se navíc připravit na velkorysé prostory, chválené občerstvení a zajímavé diskuze.

My se zase připravujeme i na možnost, že nám do cesty opět vstoupí Covid. Prostory na to budou připravené a v případě nejvyšší nouze se pravděpodobně u všech školení budeme umět přepnout do online režimu.

[![Školení ze Vzhůru dolů](https://mcusercontent.com/d6be2f1899eba6a7651157403/images/55fc0b22-7c36-4eab-b040-a4da89e3bdc8.jpg)](https://www.vzhurudolu.cz/kurzy/prezencni)

Brno:

* (Vyprodáno) [Optimalizace rychlosti webu](https://www.vzhurudolu.cz/kurzy/rychlost-nacitani) – st 7. 10.
* [Organizace CSS kódu](https://www.vzhurudolu.cz/kurzy/css-kod) (BEM, ITCSS, Suit CSS…) — út 13. 10.
* [Od dokumentace k systémům designu](https://www.vzhurudolu.cz/kurzy/dokumentace-systemy) (Jak na systémy komponent?) — st 14. 10.
* [Další…](https://www.vzhurudolu.cz/kurzy/misto-brno-superkoders)

Praha:

* [Principy JavaScriptu](https://www.vzhurudolu.cz/kurzy/javascript) (JS jako jazyk) — út 13. 10.
* [Nástroje JavaScriptu](https://www.vzhurudolu.cz/kurzy/nastroje-javascriptu) (Webpack, NPM, testování…) — st 14. 10.
* [Další…](https://www.vzhurudolu.cz/kurzy/misto-praha-greenpoint)

<br>

💰 Pokud byste se chtěli přihlásit na více školení či webinářů najednou a rovnou dostat 10 % slevu, využijte novinku — [hromadnou objednávku](https://www.vzhurudolu.cz/kurzy/hromadna-objednavka).

<br>

## 7 frontendových tipů

1. [Obrázek, který je zároveň validní JavaScript](https://dev.to/sebastianstamm/this-image-is-also-a-valid-javascript-file-5fol).
2. Vzhůru dolů podcast: [Backend vs. frontend](https://www.vzhurudolu.cz/podcast/178-frontend-backend)
3. [Neduplikujte konstanty mezi CSS a JS](https://levelup.gitconnected.com/stop-duplicating-constants-between-js-and-css-40efd253a945).
4. Vzhůru dolů: [CSS vlastnost contain](https://www.vzhurudolu.cz/prirucka/css-contain).
5. [Plyr](https://plyr.io/). Stylovatelný přehrávač videa.
6. Vzhůru dolů: [AMP weby jsou rychlé, ale můžete je špatně změřit](https://www.vzhurudolu.cz/prirucka/amp-faze).
7. [Únikovka napsaná jen pomocí CSS](https://codepen.io/takaneichinose/pen/YzqreVp?editors=0000). Vyhrajete?

Přeji vám hezké a zdravé září!

Martin Michálek