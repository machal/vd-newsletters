# Nadpis newsletteru

Hlavní text newsletteru...

---

## Rychlé tipy a&nbsp;triky

Výběr zajímavých odkazů pro vás nachystal [Martin Pešout](http://www.twitter.com/martinpesout):

- **[The future of loading CSS.](https://jakearchibald.com/2016/link-in-body/)** Umístění `<link rel="stylesheet">` uvnitř `<head>` blokuje standardně renderování stránky. Některé prohlížeče však reagují jinak na umístění `<link>` do těla `<body>`. Postupují odshora dolu. Blokují renderování pouze části obsahu, dokud není načtený aktuálně nalezený CSS soubor. Umožní ale vykreslit vše před právě načítaným `<link>`. Tato vlastnost doposud chyběla v Chrome. Nově by se toto mělo změnit.
- **[300ms zpoždění už nemusí být problémem.](https://gist.github.com/gajus/bbf06ea2e37047b01e70)** Mobilní zařízení čekají 300ms po dotyku prstu na displeji, aby zjistili, zda uživatel nechtěl udělat dvojí poklepání. Toto nepříjemné zpoždění jde odstranit např. užitím JS knihovny [Fastclick](https://github.com/ftlabs/fastclick). Čisté CSS řešení pomocí vlastnosti `touch-action` nemělo dobrou podporu mezi prohlížeči. Nově přibyla podpora i v Safari. Dokážeme tak konečně pokrýt všechny velké prohlížeče.
- **[Awesome CSS.](https://github.com/sindresorhus/awesome)** Seznam nástrojů a technik, které momentálně "frčí" mezi frontendisty.
- **[Jak na React (česky).](https://github.com/petehunt/react-howto/blob/master/README-cs.md)** Pokud jste se rozhodli začít s Reactem, lehce se můžete v celém ekosystému nástrojů a technik ztratit. Vojtěch Mikšů stál u zrodu tohoto nástroje. Zde je jeho návod popisující, co vše by měl vývojář zvládnout, aby dokázal React efektivně využít.
- **[CSS @keyframes preview in Chrome.](https://twitter.com/ChromeDevTools/status/694966453376675840)** Chrome DevTools již nějakou dobu umožňuje ladit průběh jednoduchých CSS transformací. Brzo pomocí něho dokážete upravit i jednotlivé kroky `@keyframes`.
- **[Preload: What Is It Good For?](https://www.smashingmagazine.com/2016/02/preload-what-is-it-good-for/)** `<link rel="preload">` je nový sandard, který se zaměřuje na zlepšení výkonu webů. Umožňuje vývojářům definovat vlastní logiku jak nahrávat obsahu. Dokážete tak načíst data dříve, než je prohlížeč bude skutečně potřebovat.
- **[Safari Responsive Design Mode.](http://www.macobserver.com/tmo/article/safari-9-using-responsive-design-mode)** Prohlížeč Safari můžete nově přepnout do tzv. *Reagujícího návrhového režimu*. Dokážete si tak prohlédnout, jak by váš web vypadal na iPhone, iPad, na zařízeních s Retina displejem, ale také třeba monitorech s rozlišením 1920x1080.
- **[State of email report.](https://litmus.com/lp/2016-state-of-email-report)** V průběhu roku 2015 vzrostl počet přečtených emailů na mobilních zařízeních o 17%. Nyní představuje 55% ze všech otevřených emailů. Je tedy zřejmé, že se dnes již nevyplácí podceňovat tvorbu responsivních emailů.

---

## Co jsem psal na Vzhůru&nbsp;dolů?

Seznam věcí na VD

Ať vám to dobře kóduje i v březnu!

Martin Michálek ([@machal](http://www.twitter.com/machal))

<small>PS: Hlásím zvýšenou aktivitu na Google+. Zase to s ním zkouším. :) Odebírat tam můžete přímo  [Vzhůru dolů](https://plus.google.com/b/109221560773963108322/+VzhurudoluCz/posts) nebo [můj osobní profil](https://plus.google.com/u/0/+MartinMich%C3%A1lek).</small>
