# Cvičení 2 - Zvířata

Vyzkoušej si, jak funguje v Reactu práce s obrázky ve složce `assets`.

1. Známým postupem si založ nový React projekt pomocí `create-czechitas-app` a nazvi ho třeba `zvirata`.

2. Ve složce `src` uvnitř projektu si vytvoř složku `assets`. Stáhni si [ZIP s připravenými obrázky](https://github.com/Czechitas-React-podklady/React-lekce-04/raw/main/cviceni-03-zvirata/zvirata-podklady.zip) a obrázky ze ZIPu zkopíruj do vytvořené složky `assets`.

3. V samostatné složce vytvoř komponentu `Animal`, která bude generovat následující jednoduchý kód:

	```jsx
	<div className="animal">
		<img src="ikona.jpg" alt="zvíře">
		Zvíře obecné
	</div>
	```

4. Komponenta by měla přijímat dvě props: `name` a `species`. **Name** bude název zvířete (např. *Slon africký*), **species** bude obsahovat "typ" zvířete (např. *slon*)

	Používej pouze následující typy, protože pro ně máme připravené obrázky:

	```
	gibon
	lev
	nosorozec
	panda
	papousek
	slon
	surikata
	tygr
	velbloud
	zirafa
	```

5. V komponentě zařiď, aby se zobrazil správný obrázek podle předaného druhu zvířete. Tj. když bude v `species` hodnota `papousek`, měl by se zobrazit obrázek `papousek.jpg` ze složky `assets`.

6. V komponentě `App` zkus komponentu několikrát použít pro různá zvířata, abys ověřila, že vše správně funguje.

7. Pokud se nudíš, nastyluj komponentu tak, aby stránka vypadala hezky.
