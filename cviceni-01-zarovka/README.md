# Cvičení 1 - Žárovka

Vytvoř aplikaci s komponentou `Bulb`, která se podle předaných props buď rozsvítí nebo zhasne.

1. Založ si nový React projekt pomocí `create-czechitas-app` a nazvi ho třeba `zarovka`. Vymaž výchozí obsah ukázkové aplikace.

1. V **samostatné složce** vytvoř novou komponentu `Bulb`. Její obsah bude jednoduchý, půjde pouze o jeden `<div>` s CSS třídou `bulb`.

	```html
	<div className="bulb"></div>
	```

1. Stáhni si [ZIP s připravenými styly a obrázky](https://github.com/Czechitas-React-podklady/React-lekce-04/raw/main/cviceni-01-zarovka/zarovka-zadani.zip) pro rozsvícenou a zhasnutou žárovku a přidej je do složky komponenty `Bulb`.

	Styly týkající se konrétně žárovky nech v CSS souboru komponenty. Styly týkající se stránky (html, body, apod.) ze souboru vyjmi a přepiš jimi obsah hlavního CSS souboru `style.css` naší aplikace.

1. Když prozkoumáš připravené styly pro žárovku, tak uvidíš, že CSS třída `bulb` standardně zobrazuje zhasnutou žárovku. Teprve když divu **přidáš ještě druhou** třídu nazvanou `bulb--on`, tak se obrázek s žárovkou změní na rozsvícenou žárovku.

1. Použij komponentu `Bulb` a zobraz ji na stránce (tj. vlož ji do komponenty `App`).

1. Chceme zařídit, že pokud komponentu použijeme takto, zobrazí se zhasnutá žárovka:
	```jsx
	<Bulb on={false} />
	```

	Pokud ji naopak použijeme takto, žárovka se zobrazí rozsvícená:

	```jsx
	<Bulb on={true} />
	```
	nebo prostě takto
	```jsx
	<Bulb on />
	```

 	Kýženého chování dosáhnete tak, že sestavíte obsah atributu `className` našeho divu s žárovkou pomocí ternárního operátoru v závislosti na hodnotě v prop nazvané `on`.

1. Vlož na stránku zhasnutou i rozsvícenou žárovku.
