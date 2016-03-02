# Webařův checklist teď i jako&nbsp;aplikace

Proč dělat weby blbě, když je můžete dělat dobře? Třeba podle [kontrolního seznamu ze Vzhůru dolů](http://www.vzhurudolu.cz/checklist).

[![Checklist pro dokončení webu](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/9d3a7d0e-c377-4156-8ddd-a912ff462ddb.jpg)](http://www.vzhurudolu.cz/checklist)

Webařův checklist měl v [podobě článku a PDF](http://www.vzhurudolu.cz/prirucka/checklist) hezké ohlasy. Jenže… *Článek*  v době, kdy existují aplikace snad i na drbání za uchem!? *Pé dé ef*  ve století, ve kterém všechny potíže světa vyřešil React?!

Já vím, já vím. Obojí je trochu nepraktické. A proto vznikla tahle miniaplikace. Nejlepší bude, když si ji prostě otevřete:

<p class="text-center">
<a href="http://www.vzhurudolu.cz/checklist" class="button">Vyzkoušet checklist</a>
</p>

Funguje tak, jak asi očekáváte:

- Prok každý projekt si vytvoříte nový seznam a případně jej nasdílíte s kolegy.
- Přidáváte, upravujte nebo mažete položky seznamů.
- My vám budeme ukládat průběžný stav plnění úkolů na serveru, abyste to měli dostupné ze všech zařízení.

Hlavní cílovou skupinou jsou frontend kodéři. Největší využití checklist najde pro dokončovací práce na statických webech. Je v něm ale řada překryvů do backendu i dalších webařských řemesel. Zkuste si to.

Nápady a připomínky k funkčnosti i obsahu velmi vítám. Odpovězte na tento email nebo prostě napište na [martin@vzhurudolu.cz](mailto:martin@vzhurudolu.cz).

---

## Šest krátkých odkazů jinam

Výběr zajímavých odkazů pro vás nachystal [Martin Pešout](http://www.twitter.com/martinpesout):

- **[The future of loading CSS.](https://jakearchibald.com/2016/link-in-body/)** Chrome mění chování `<link rel="stylesheet">`, pokud ho umístíte uvnitř `<body>`. Tam dostane chování podobné `<script>` – vykreslí se část nad ním, čeká se na stažení CSS a pak se vykreslí část pod ním. Stránka se bude zobrazovat postupně po komponentách a uživatel nebude muset čekat na načtení všech CSS souborů. 
- **[Už brzy nebudeme muset řešit 300ms zpoždení prokliků Javascriptem.](https://gist.github.com/gajus/bbf06ea2e37047b01e70)** Nepříjemné zpoždění znají uživatelé dotykových zařízení. Je způsobeno tím, že prohlížeč čeká, zda uživatel nechtěl udělat dvojklik. Prodlevu lze odstranit např. pomocí JS knihovny [Fastclick](https://github.com/ftlabs/fastclick). Máme tu ale i řešení čistě pomocí CSS – `touch-action`. Chybějící podpora v Safari má zmizet s příchodem nové verze. Bude tak konečně možné pokrýt všechny velké prohlížeče.
- **[Awesome CSS.](https://github.com/sindresorhus/awesome)** Opravdu úžasný seznam nástrojů a technik, které momentálně „frčí“ mezi frontendisty.
- **[Jak na React (česky).](https://github.com/petehunt/react-howto/blob/master/README-cs.md)** Pokud jste se rozhodli začít s Reactem, lehce se můžete v celém ekosystému nástrojů a technik ztratit. Vojtěch Mikšů přeložil do češtiny návod popisující, co vše by měl vývojář zvládnout, aby dokázal React efektivně využít.
- **[CSS @keyframes preview in Chrome.](https://twitter.com/ChromeDevTools/status/694966453376675840)** Chrome DevTools již nějakou dobu umožňuje ladit průběh jednoduchých CSS transformací. Brzo v něm bude možné upravit i jednotlivé kroky `@keyframes`.
- **[Preload: What Is It Good For?](https://www.smashingmagazine.com/2016/02/preload-what-is-it-good-for/)** `<link rel="preload">` je nový sandard, který se zaměřuje na zlepšení rychlosti načítání webů. Umožňuje vývojářům definovat vlastní logiku nahrávání obsahu. Načte data dříve, než je prohlížeč bude potřebovat k vykreslení.

---


[![Školení SVG, Javascriptu a Bootstrapu](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/d55ab17d-2ab7-4cd2-a83c-c9d504e9aecd.png)](http://www.vzhurudolu.cz/kurzy)

V plánu máme tři školení:

* [Scalable Vector Graphics alias SVG](http://www.vzhurudolu.cz/kurzy/svg) s Michalem Matuškou. Od jednoduchých využití vektorů až po animace, efekty a interaktivní infografiky. Na [15. března](http://www.vzhurudolu.cz/kurzy/svg) hlásíme poslední tři místa.
* [Principy Javascriptu](http://www.vzhurudolu.cz/kurzy/javascript) vám přiblíží Riki Fridrich. Naučte se Javascript jako jazyk konečně pořádně.  Další termín je [22. března](http://www.vzhurudolu.cz/kurzy/javascript).
* [Bootstrap](http://www.vzhurudolu.cz/kurzy/bootstrap) a jeho rozšiřování učí Adam Kudrna, autor pokročilé (a moc pěkné!) prototypovací nástavby Bootstrapu, [Synergic UI](http://ui.synergic.cz/).  Přihlaste se na [24. března](http://www.vzhurudolu.cz/kurzy/bootstrap).

Nezapomeňte – každý z kurzů můžete [objednat také jako školení do firmy](http://www.vzhurudolu.cz/kurzy#inhouse).

---

## Co jsem psal na Vzhůru&nbsp;dolů?

- **[Vše o meta značce pro viewport](http://www.vzhurudolu.cz/prirucka/viewport-meta)**. Znáte ji, já vím. Ale zároveň se vsadím, že o ní ještě nevíte všechno.
- **[Proč řešit rychlost načítání webů?](http://www.vzhurudolu.cz/prirucka/rychlost-nacitani-proc)**. Košík plný argumentů. Doporučuji ještě před obědem servírovat šéfovi, klientům a ukázat i kolegům designérům a grafikům. Bez jejich přesvědčení dělat rychlejší weby nejde.

To by už stačilo, protože „březen, za kamna vlezem a pár webů nakódujem“!

Zdraví vás

Martin Michálek ([@machal](http://www.twitter.com/machal))
