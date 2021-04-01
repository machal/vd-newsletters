## Milé čtenářky, milí čtenáři,

doufám, že se máte v rámci možností dobře. Ve 41. vydání newsletteru ze Vzhůru dolů, které právě čtete, mírně měním formát. Snad se vám bude líbit. Za váš názor budu vděčný, stačí odpovědět na tento e-mail. 😊

## Jak zrychlit web v roce 2021?

Page Experience update od Googlu, který bude klást větší důraz na rychlost, se blíží, a tak se v dnešním newsletteru pojďme zaměřit na to, co je mi odborně nejbližší – na rychlost.

V následujícím seznamu nemám ambici být obsahově vyčerpávající, spíše připomínám metody, které jsou relativně nové, které se mi osvědčily, a o kterých jsem psal [na Vzhůru dolů](https://www.vzhurudolu.cz/), kde také vyjde rozšířená verze tohoto textu.

Předpokládám, že základy znáte. Že zmenšujete datový objem, snižujete počet requestů, máte nasazené [HTTP/2](https://www.vzhurudolu.cz/prirucka/http-2) a tak dále. Pojďme na to.

### 1) Dobře měřte

Nezapomeňte, že [Lighthouse score](https://www.vzhurudolu.cz/prirucka/metrika-lps) neudává rychlost webu. Jen zhruba indikuje, kolik problémů na webu máte. Dívejte se na data od uživatelů – z [Chrome UX Reportu](https://www.vzhurudolu.cz/prirucka/chrome-ux-report). Vývoj v čase uvidíte v měření [PageSpeed.cz](https://pagespeed.cz/).

### 2) Metriky? Zaměřte se na Web Vitals

[Metrik rychlosti](https://www.vzhurudolu.cz/prirucka/metriky-rychlosti) je opravu hodně, pro různé projekty se hodí různé ukazatele. V prvé řadě se zaměřte na [Core Web Vitals](https://www.vzhurudolu.cz/prirucka/web-vitals): [LCP](https://www.vzhurudolu.cz/prirucka/metrika-lcp), [FID](https://www.vzhurudolu.cz/prirucka/metrika-fid), [CLS](https://www.vzhurudolu.cz/prirucka/metrika-cls).

### 3) Lazy loading dejte skoro všude

[Líné načtení](https://www.vzhurudolu.cz/prirucka/lazy-loading-obrazku) pro `<img>` nebo `<iframe>` opravdu pomůže. Sníží datový objem stránky, vylepší prioritizaci zdrojů. Líně ale nenačítejte zdroje důležité pro první viewport.

[![Webinář o lazy loadingu](https://mcusercontent.com/d6be2f1899eba6a7651157403/images/5ff0ab91-e3b4-4e1f-92aa-4714bb2244c3.png)]((https://www.vzhurudolu.cz/kurzy/webinar-lazy-loading))

👉  **Tip:** Na tohle téma chystám [ve středu 7. 4. webinář](https://www.vzhurudolu.cz/kurzy/webinar-lazy-loading), kde se na líné načtení (ale také línou evaluaci a líný rendering) podíváme detailně.

### 4) Nepoužívejte CDN pro kritické zdroje

Díky přechodu Chrome na [partitioned (dělenou) cache](https://www.vzhurudolu.cz/prirucka/partitioned-cache), přestaly CDN dávat smysl pro sdílení zdrojů mezi weby. Zdroje kritické pro první vykreslení na externí CDN raději nedávejte.

### 5) Preconnect pro kritické zdroje

[Včasné připojení](https://www.vzhurudolu.cz/prirucka/preconnect) pomocí `<link rel=preconnect>` může stránku urychlit, pokud jsou kritické zdroje uložené na jiných doménách. Nepoužívejte to ale na všechny domény, kde jsou uložené zdroje stránky, například u analytiky to většinou smysl nedává.

### 6) Preloadujte, ale šetřete s tím

`<link rel=preload>` může opravdu hodně pomoci, hlavně s metrikou LCP. Jenže zpravidla řeší problém, který vznikl špatným nakódovaním stránky. A může přinést problémy nové. Přemýšlejte, než [přednačtení](https://www.vzhurudolu.cz/prirucka/preload) nasadíte. Je to hack a může to být past.

👉  **Tip:** O preload mluvím [na videu z webináře o metrice LCP](https://www.vzhurudolu.cz/video/webinar-lcp).

### 7) Využijte nové formáty obrázků: AVIF, WebP

Formát [WebP](https://www.vzhurudolu.cz/prirucka/webp) jde použít už ve všech moderních prohlížečích. Jděte do toho. Experimentujte také s famózně úsporným [AVIF](https://www.vzhurudolu.cz/prirucka/avif).

### 8) Držte layout

Optimalizace pro metriku Cumulative Layout Shift vyžaduje, abyste asynchronním prvkům jako jsou obrázky nebo externí zdroje drželi prostor v rozvržení. U [obrázků](https://www.vzhurudolu.cz/prirucka/img-pomer-stran) je to už poměrně snadné, jinde pomůže nová [metoda](https://www.vzhurudolu.cz/prirucka/css-aspect-ratio) s funkcí aspect-ratio() nebo starší [triky](https://www.vzhurudolu.cz/prirucka/css-pomer-stran).

👉  **Tip:** O metrice CLS mám také [video z webináře](https://www.vzhurudolu.cz/video/webinar-cls) a lidé říkají, že je bezva.

## Co je nového na Vzhůru dolů?

1. **Layout, všude samý layout.** Razantně jsem aktualizoval příručku [o flexboxu](https://www.vzhurudolu.cz/prirucka/css-flexbox). Spolu [s gridem](https://www.vzhurudolu.cz/prirucka/css-grid), [zarovnáváním boxů](https://www.vzhurudolu.cz/prirucka/css-box-alignment) a [vícesloupcovým layoutem](https://www.vzhurudolu.cz/prirucka/css-multicolumn) je k dispozici všem, které zajímají nové layouty v CSS.
2. S Veronikou Bedáňovou jsme připravili **případovou studii [o přístupnosti na Rohlík.cz](https://www.vzhurudolu.cz/blog/190-pristupnost-rohlik)**.
3. **Freelancer Metuzalém.** U příležitosti rozhovoru pro portál Na volné noze jsem připravil text [20 let na volné noze](https://www.vzhurudolu.cz/blog/192-volna-noha-20). Zavzpomínal jsem si. Ale snažil se to psát velmi otevřeně a tak, aby text mohl být užitečný pro každého, kdo volnou nohu zvažuje. Nebo pokud vás jen zajímá, jaké přemýšlení za Vzhůru dolů stojí.
4. **[Knihy](https://www.vzhurudolu.cz/prirucka/knihy)** pro frontendisty a frontendistky. Taky milujete papír?
5. S Robinem jsme natočili **dva podcasty**. O stavu CSS/JS [s Rikim Fridrichem](https://www.vzhurudolu.cz/podcast/188-state-of-fczbkk-2020) a o mezinárodním freelancingu a AR/VR [s Evou Kuttichovou](https://www.vzhurudolu.cz/podcast/193-podcast-eva-kuttichova).
6. Do **[sekce video](https://www.vzhurudolu.cz/video)** přibyly tři nové minikurzy: o metrikách LCP, CLS a vkládání SVG na web. Už tady máme 18 videí, takže je z čeho vybírat.

[![Nová videa](https://mcusercontent.com/d6be2f1899eba6a7651157403/images/5ff0ab91-e3b4-4e1f-92aa-4714bb2244c3.png)](https://www.vzhurudolu.cz/video)

## Tipy odjinud

1. [Adee](https://www.adeeapp.com/). Plugin pro testování přístupnosti už ve Figmě nebo Sketchi.
2. V CSS se chystá [nativní zanořování selektorů](https://benfrain.com/official-css-nesting-the-last-piece-of-the-puzzle/).
3. [HTML over WebSockets](https://alistapart.com/article/the-future-of-web-software-is-html-over-websockets/). Zpět ke spásnému backendu? Nebo zpět na stromy?
4. Lea Verou: [Dark Mode in 5 minutes](https://lea.verou.me/2021/03/inverted-lightness-variables/).
5. CSS Tricks: [Nástroje pro audit CSS](https://css-tricks.com/tools-for-auditing-css/).

Přeji vám krásný začátek jara!

Martin Michálek