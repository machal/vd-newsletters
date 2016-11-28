# HTTP/2: Které české hostingy ho podporují?

Vítám vás u dalšího vydání newsletteru ze Vzhůru dolů!

Zjišťoval jsem nedávno, jak jsme na tom v Česku [s HTTP/2](http://www.vzhurudolu.cz/prirucka/http-2), novým rychlým protokolem, který pomůže weby velmi zrychlit. Pár webů už na něm tady běží a pokud máte vlastní server, doporučuji si tam nechat podporu zapnout. 

Na sdíleném hostingu je to horší. Ty české většinou čekají na stabilní verzi [mod_http2](https://httpd.apache.org/docs/2.4/mod/mod_http2.html). Na [cn130.com](http://cn130.com/2015/12/webhosting-s-http-2-0/) je pěkný seznam českých hostingů, které HTTP/2 podporují. Tedy seznam… Jsou zatím tři. Možná.

- [Wedos](https://hosting.wedos.com/cs/newsletters/2016/05/01.html) prý podporuje HTTP/2 u všech linuxových tarifů.
- [Active24](https://www.active24.cz/) mě napsali, že [HTTP/2 umí na všech tarifech](https://www.facebook.com/active24cz/posts/10211267842150771), což je cool. Škoda jen, že aktuálně to nejspíš využijí jen vaší uživatelé s Firefoxem.
- [Tele3](https://www.tele3.cz/) to prý nastavuje na vyžádání.

Vyjádření [z Ignum](https://twitter.com/ignum/status/801353087189454848):

> Současná stabilní verze platformy Debian/apache, kterou používáme, HTTP/2 nepodporuje. S přechodem na Debian 9 s HTTP/2 počítáme.

V podobném duchu mě psal Matěj Kloubek z [Českého hostingu](http://www.cesky-hosting.cz/):

> Experimentální věci samozřejmě nechceme na servery nasazovat, protože jednak není jisté, že budou správně fungovat, a taky se ještě mohou dost měnit. Takže čekáme, až ten modul bude vydán jako stabilní (a to jak obecně, tak pro Debian).

Vývoj budu sledovat. Pokud víte o podpoře u jiných hostingů, napište mi prosím. Pokud váš hosting HTTP/2 podporuje, jděte do toho. Více [o HTTP/2 je na Vzhůru dolů](http://www.vzhurudolu.cz/prirucka/http-2).

---

## Sleva za včasnou  objednávku školení

[![Včasná objednávka školení](https://gallery.mailchimp.com/d6be2f1899eba6a7651157403/images/ea58b241-0054-44a2-896a-c848715df722.jpg)](http://www.vzhurudolu.cz/kurzy)

Mám už vypsané jarní termíny svých školení a vy můžete ušetřit. Běžná cena je 4&nbsp;490 Kč bez DPH, Early Bird cena pak 3&nbsp;900 Kč. Ušetříte tedy 590 Kč bez DPH. Sleva platí do 16. prosince.

Slevový kupón můžete uplatit pro tato školení:

- [Dnešní webová kodéřina](http://www.vzhurudolu.cz/kurzy/webova-koderina) (23. 2.)
- [Responzivní design](http://www.vzhurudolu.cz/kurzy/responzivni-design) (9. 3.)
- [Rychlost načítání](http://www.vzhurudolu.cz/kurzy/rychlost-nacitani) (23. 3.)

V objednávce uveďte kód `EARLY2017`.

---


## Co zajímavého psali jinde?

- [How To Poison The Mobile User](https://www.smashingmagazine.com/2016/10/how-to-poison-the-mobile-user/). Jak otrávit mobilního uživatele. Aneb co určitě nedělat v rozhraní responzivních webů. Autora znáte, vsaďte se. ;)
- [Position: sticky se vrací do Chrome](https://www.chromestatus.com/feature/6190250464378880). Přistane už velmi brzy, do verze 56. [Je to hybrid](https://developer.mozilla.org/en-US/docs/Web/CSS/position#Sticky_positioning) mezi relativní a fixní pozicí a hodí se na pěkné věci, které znáte z nativních aplikací. Zatím si dema prohlížejte ve Firefoxu. S rozumným fallbackem pro starší prohlížeče rozhodně [použitelné už dnes](http://caniuse.com/#search=position%3Asticky). 
- [Rozcestník odkazů o progresivních webových aplikacích](https://dev.opera.com/articles/pwa-resources/). Webových apkách, které mají vlastnosti nativních.
- [CSS Grid, Flexbox a Box Alignment](https://www.smashingmagazine.com/2016/11/css-grids-flexbox-and-box-alignment-our-new-system-for-web-layout/) v podrobném článku od Rachel Andrew, která o nich přednášela na letošním [WebExpu](https://webexpo.cz/praha2016/prednaska/the-right-layout-tool-for-the-job/). Příští rok už v našich prohlížečích.
- [Jak pomocí PostCSS a CSSnext nahradit základní vlastnosti preprocesorů](https://www.sitepoint.com/future-css-with-postcss-cssnext/). Hlavně proměnné nebo mixiny.
- [Budoucnost responzivního designu](https://medium.com/@unakravets/rethinking-responsive-d557ef1745bd). Pěkné věci nás čekají. WebVR, geolokace, physical web, battery level, ambient light queries…

---

## Vzhůru do lepší práce

- [**Ataccama** – React/Elm Developera](https://jobs.ataccama.com/react-elm-developer) (Praha)
- [**Ataccama** – Frontend Architect](https://jobs.ataccama.com/front-end-architect) (Praha)

Děkuji tímto Ataccamě, partnerovi [sekce s pracovní inzercí](http://www.vzhurudolu.cz/prace).

---

## Co je nového na Vzhůru dolů? Podcast!

- [Vzhůru dolů podcast](http://www.vzhurudolu.cz/blog/74-podcast-robin-berlin). Natočil jsem první díl s Robinem Pokorným o Berlíně. Jablíčkáři, odebírejte [tady](https://itunes.apple.com/cz/podcast/vzhuru-dolu-podcast/id1176274658), ostatní [tady](https://soundcloud.com/vzhurudolu). 
- [Atomický design a Pattern Lab](http://www.vzhurudolu.cz/prirucka/pattern-lab). Systémy designu. Téma, kterému se budu dále věnovat, protože mě v praxi hodně baví.
- [Hluboká práce: jak dělat více lepších věcí](http://www.vzhurudolu.cz/blog/75-hluboka-prace). Kdy jste naposledy měli půldne času na pořádnou práci a bez jediného vyrušení? Že si nevzpomínáte? Pak čtěte.
- [Majitelé „m tečka“ webů pozor: Google bude mobile-first](http://www.vzhurudolu.cz/blog/73-google-mobile-first). Pokud ale máte responzivní web, nijak vám to vadit nebude.

---

Přeji vám co nejméně hektické předvánoční období a hezké svátky!

Martin Michálek
[vzhurudolu.cz/martin](http://vzhurudolu.cz/martin)

