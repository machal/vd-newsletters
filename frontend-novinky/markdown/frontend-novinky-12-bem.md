# BEM CSS: Jak se vyhnout častým problémům?

David Berner v bezva článku [na Smashing Magazine](https://www.smashingmagazine.com/2016/06/battling-bem-extended-edition-common-problems-and-how-to-avoid-them/) bojuje s častými problémy při používání [BEM](http://www.vzhurudolu.cz/prirucka/bem), metodiky pro pojmenovávání tříd v CSS.

Dovolil jsem si některé problémy ořezat na kost a doplnit svými komentáři.  Budeme si povídat o nešvarech jako je přenášení struktury dokumentu do CSS, o lásce k ampersandům, křížení komponent a responzivních příponách.

## DOM struktura v CSS místo nemá

Takhle ne:

```
<div class="card">
  <div class="card__header">
    <h2 class="card__header__title">…</h2>
  </div>
</div>
```

Takhle ano:

```
<div class="card">
  <div class="card__header">
    <h2 class="card__title">…</h2>
  </div>
</div>
```

Zanořování elementů i v selektorech by se vám totiž dříve nebo později vymklo z rukou. BEM třídy nepatří k nejkratším. Nevytvořte si z nich Frankensteina řetězením elementů. 

Obecně nemá respektování struktury DOMu v CSS žádné mě známé výhody.

## Ampersandové úlety

Takhle ne:

```
.card {
  &__header { … }
  &__title { … }
}
```

Takhle ano:

```
.card__header { … }
.card__title { … }
```

Na příkladu to není moc vidět, ale představte si opravdu dlouhý seznam deklarací zanořených do `.card`. A teď si představte, jak snadno někde uprostřed ztratíte jistotu co vlastně onen ampersand představuje. 

Připadá vám blbé psát `.card` pořád dokola? To pozor, kód nepíšeme proto, aby se nám dobře *psal*, ale dobře *četl*. A rozumný editor kódu nám s otravným psaním vždycky pomůže.

## Křížení nechte rostlinářům, u komponent jej nezkoušejte

Takhle ne:

```
<div class="card">
  <button class="button card__button">…</button>
</div>
```

Takhle ano:

```
<div class="card">
  <button class="button button--small">…</button>
</div>
```

Pomocí `.card__button` modifikujeme blok `.button`  uvnitř bloku `card`. Jenže pozor! Děláme to v nové komponentě, kde na očích nemáme původní kód a může se nám snadno stát, že použití v HTML selže například při nedodržení pořadí tříd.

Pro mě užitečný postřeh, protože dosud jsem vehementně křížil a nevýhody mně nedocházely.  

## Responzivní přípony

Stalo se vám, že na malém displeji chcete obsah zobrazit jako seznam položek a na velkém jako karusel? Uděláte to snadno pomocí responzivních zavináčových přípon:

```
<ul class="c-image-list@small-screen c-carousel@large-screen">
```

Tohle je [další z příspěvků](http://csswizardry.com/2015/08/bemit-taking-the-bem-naming-convention-a-step-further/) od Harryho Robertse, které jsem neznal a za které děkuji. 

Co vy na to? Napadnou vás další BEM nešvary? Jsem na ně zvědavý. Stačí odpovědět na  e-mail. ;)

---

## Odkazy jinam: HTML hlavičky, krásně napsané komponenty, autofill…

- **[Co všechno můžete přidat do HTML hlavičky?](https://github.com/joshbuchea/HEAD)** Je toho tolik, že vás asi rozbolí `<head>`. Nezapomeňte, že ty nejpodstatnější meta značky jsou ve [webařově checklistu](http://www.vzhurudolu.cz/prirucka/checklist).
- **[Frend, správně udělané komponenty.](http://frend.co/)** Kolekce krásně nakódovaných komponent typu záložky, modály, tooltipy… Ošetřená přístupnost, žádné závislosti na jQuery. CSS v BEM názvosloví. Skvělé!
- **[Vše o autofill.](http://blog.cloudfour.com/autofill-what-web-devs-should-know-but-dont/)** Píše Jason Grigsby. Věděli jste třeba, že mobilní Safari umí naskenovat údaje z fyzické platební karty? Jen k tomu nikde není dokumentace.
- **[Stylelint, linting pro CSS.](https://www.smashingmagazine.com/2016/05/stylelint-the-style-sheet-linter-weve-always-wanted/)** Na Smashing Magazine píšou, že je takový jaký jsme vždycky chtěli. A opravdu tak vypadá. 
- **[Tachyons](http://tachyons.io/)** je natolik jiný CSS framework, že hledám slova. Anti-komponentový?
- Inspirace: **[Jak hudba ovlivňuje produktivitu?](https://medium.com/life-learning/how-music-affects-your-productivity-42a6dfa6fdfe#.v81m677en)** Ambientní plochy startují kreativitu. Když se chcete soustředit, pusťte si hudbu co dobře znáte a ideálně beze slov, kterým byste nedejbože mohli rozumět. Nejvíce vás práce pohltí, když si pustíte klasiku nebo třeba soundtracky ke hrám.

---

## Co je nového na Vzhůru dolů? 

- Napsal jsem případovku k aktuální klientské práci. **[Jaký vliv má zrychlení webu na konverzní poměr?](http://www.vzhurudolu.cz/blog/58-rychlost-srovname-cz)** U Srovname.cz na mobilech vyrostl o čtvrtinu.
- **[11 tipů pro Bootstrap, které jste možná neznali.](http://www.vzhurudolu.cz/blog/60-bootstrap-tipy)** Co třeba Bootlint validátor? A vyznáte se v centrování?
- **[CSS řešení: hlavička s videem na pozadí.](http://www.vzhurudolu.cz/blog/59-css-video-hlavicka)** Konkrétní kodérský problém rozpitvaný do detailu. Používám flexbox, vh jednotky a další.

Na závěr – prosím vás, pošlete své profesní kamarády, který by se moje newslettery mohly líbit na **[novou stránku pro přihlášení k newsletterům](http://www.vzhurudolu.cz/email)**. Nebo jim prostě přepošlete tenhle. Díky! ;)

Hezké léto přeje

Martin Michálek
[vzhurudolu.cz/martin](http://vzhurudolu.cz/martin)

<small>PS: V létě si dáme newsletterovou přestávku. Tedy s jedinou výjimkou - novinkou na webu, kterou brzy ohlásím. Zprávičky kolem frontend tématiky ale budou dále vycházet [na Facebooku](https://www.facebook.com/vzhurudolu) a [Twitteru](https://twitter.com/vzhurudolu). ;)</small>