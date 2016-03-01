# Webařův checklist teď i jako&nbsp;aplikace

Proč dělat weby blbě, když je můžete dělat dobře? Třeba podle [kontrolního seznamu ze Vzhůru dolů](http://www.vzhurudolu.cz/checklist).

[![Checklist pro dokončení webu](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/9d3a7d0e-c377-4156-8ddd-a912ff462ddb.jpg)](http://www.vzhurudolu.cz/checklist)

Webařův checklist měl v podobě článku nebo PDF hezké ohlasy. Jenže… *Článek*  v době, kdy existují aplikace snad i na drbání za uchem!? *Pé dé ef*  ve století, ve kterém všechny potíže světa vyřešil React?!

Já vím, já vím. Obojí je trochu nepraktické. A proto vznikla tahle miniaplikace. Jděte si ji hned zkusit:

<p class="text-center">
<a href="http://www.vzhurudolu.cz/checklist" class="button">Vyzkoušet checklist</a>
</p>

Funguje to tak, jak asi očekáváte:

- Vytvoříte si nový seznam a případně jej nasdílíte s kolegy.
- Přidáváte, upravujte nebo mažete položky seznamů.
- My vám budeme ukládat průběžný stav plnění úkolů na serveru, abyste to měli dostupné ze všech zařízení.

Hlavní cílovou skupinou jsou frontend kodéři. Největší využití checklist najde pro dokončovací práce na statických webech. Je v něm ale řada překryvů do backendu i dalších webařských řemesel. Zkuste si to.

Nápady a připomínky k funkčnosti i obsahu velmi vítám. Odpovězte na tento email nebo prostě napište na [martin@vzhurudolu.cz](mailto:martin@vzhurudolu.cz).

---

## Rychlé tipy a&nbsp;triky

Výběr zajímavých odkazů pro vás nachystal [Martin Pešout](http://www.twitter.com/martinpesout):

- **[The future of loading CSS.](https://jakearchibald.com/2016/link-in-body/)** Umístění `<link rel="stylesheet">` uvnitř `<head>` blokuje standardně renderování stránky. Některé prohlížeče však reagují jinak na umístění `<link>` do těla `<body>`. Postupují odshora dolu. Blokují renderování pouze části obsahu, dokud není načtený aktuálně nalezený CSS soubor. Umožní ale vykreslit vše před právě načítaným `<link>`. Tato vlastnost doposud chyběla v Chrome. Nově by se toto mělo změnit.
- **[Už brzy půjde řešit 300ms zpoždění prokliků jen v CSS .](https://gist.github.com/gajus/bbf06ea2e37047b01e70)** Mobilní zařízení vyčkávají 300ms po dotyku prstu na displeji, aby zjistili, zda uživatel nechtěl udělat dvojí poklepání. Toto nepříjemné zpoždění lze odstranit např. pomocí JS knihovny [Fastclick](https://github.com/ftlabs/fastclick). Existuje však i řešení čistě pomocí CSS a nazývá se `touch-action`. Jenže tato vlastnost neměla stále dobrou podporu mezi prohlížeči a chyběla podpora v Safari. To se má s příchodem nové verze. Dokážeme tak konečně pokrýt všechny velké prohlížeče.
- **[Awesome CSS.](https://github.com/sindresorhus/awesome)** Opravdu úžasný seznam nástrojů a technik, které momentálně „frčí” mezi frontendisty.
- **[Jak na React (česky).](https://github.com/petehunt/react-howto/blob/master/README-cs.md)** Pokud jste se rozhodli začít s Reactem, lehce se můžete v celém ekosystému nástrojů a technik ztratit. Vojtěch Mikšů přeložil do češtiny návod popisující, co vše by měl vývojář zvládnout, aby dokázal React efektivně využít.
- **[CSS @keyframes preview in Chrome.](https://twitter.com/ChromeDevTools/status/694966453376675840)** Chrome DevTools již nějakou dobu umožňuje ladit průběh jednoduchých CSS transformací. Brzo pomocí něho dokážete upravit i jednotlivé kroky `@keyframes`.
- **[Preload: What Is It Good For?](https://www.smashingmagazine.com/2016/02/preload-what-is-it-good-for/)** `<link rel="preload">` je nový sandard, který se zaměřuje na zlepšení rychlosti načítání webů. Umožňuje vývojářům definovat vlastní logiku jak nahrávat obsahu. Dokážete tak načíst data dříve, než je prohlížeč bude skutečně potřebovat.

---


[![Školení SVG, Javascriptu a Bootstrapu](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/d55ab17d-2ab7-4cd2-a83c-c9d504e9aecd.png)](http://www.vzhurudolu.cz/kurzy)

V plánu máme tři školení:

* [Scalable Vector Graphics alias SVG](http://www.vzhurudolu.cz/kurzy/svg) s Michalem Matuškou. Od jednoduchých využití vektorů až po animace, efekty a interaktivní infografiky. Poslední tři místa na [15. března](http://www.vzhurudolu.cz/kurzy/svg).
* [Principy Javascriptu](http://www.vzhurudolu.cz/kurzy/javascript) vám přiblíží Riki Fridrich. Javascript jako programovací jazyk konečně pořádně.  Přihlaste se na [22. března](http://www.vzhurudolu.cz/kurzy/javascript).
* [Bootstrap](http://www.vzhurudolu.cz/kurzy/bootstrap) a jeho rozšiřování ukazuje Adam Kudrna, autor pokročilé prototypovací nástavby Bootstrapu, [Synergic UI](http://ui.synergic.cz/).  Přihlaste se na [24. března](http://www.vzhurudolu.cz/kurzy/bootstrap).

Je dobré připomenout, že si každý z kurzů můžete [objednat jako školení do firmy](http://www.vzhurudolu.cz/kurzy#inhouse).

---

## Co jsem psal na Vzhůru&nbsp;dolů?

V lednu jste u nás doma mohli slyšet zvuk klávesnice v kadenci zcela neuvěřitelné. Osm článků na blogu je asi můj rekord. Pro vás vybírám ty s největším ohlasem:

- **[Vše o meta značce pro viewport](http://www.vzhurudolu.cz/prirucka/viewport-meta)**. Znáte ji, vím to. Ale vsadím se, že o ní ještě nevíte všechno.
- **[Proč řešit rychlost načítání webů?](http://www.vzhurudolu.cz/prirucka/rychlost-nacitani-proc)**. Košík plný argumentů. Doporučuji servírovat šéfovi, klientům a ukázat i kolegům.

To by už stačilo, protože „březen, za kamna vlezem a pár webů nakódujem'“!

Martin Michálek ([@machal](http://www.twitter.com/machal))
