# Cvičení 1 - Osoby

Vyzkoušej si, jak funguje v Reactu práce s naimportovanými obrázky.

1. Známým postupem si založ nový React projekt pomocí `create-czechitas-app` a nazvi ho třeba `osoby`.

2. V samostatné složce vytvoř komponentu `Person`, která bude generovat následující jednoduchý kód:

	```jsx
	<div className="person">
		<img src="ikona.jpg" alt="žena">
		Jana Nováková
	</div>
	```

4. Komponenta by měla přijímat dvě props: `name` a `gender`. **Name** bude jméno osoby, **gender** může obsahovat hodnotu `f` (female/žena) nebo `m` (male/muž).

5. Stáhni si [ZIP s připravenými obrázky](https://github.com/Czechitas-React-podklady/React-lekce-04/raw/main/cviceni-01-osoby/osoby-ikony.zip).

	Kdyby ty stejné obrázky používalo více komponent, umístili bychom je do složky `img` uvnitř složky `src` celého projektu. Protože ale naše konkrétní obrázky jsou relevantní jen pro pomponentu `Person`, bude lepší, když je umístíme přímo do složky komponenty. Ideálně si ve složce s komponentou vytvoř složku `img` nebo `images` a do ní zkopíruj obrázky ze ZIPu.

6. V souboru s komponentou naimportuj obě ikony. Podle obsahu prop `gender` (obsahuje hodnoty `f` nebo `m`) zobraz ve značce `<img />` správnou ikonu a do atributu `alt` napiš `žena` nebo `muž`.

7. V hlavní komponentě `App` použij několikrát naši komponentu `Person` a zobraz několik můžů i žen, abys vyzkoušela, že vše správně funguje.

8. Budeme se držet toho nejtrapnějšího klišé na světě a chceme, aby ženy byly podbarvené světle růžovou barvou a muži modrou. Vytvoř u komponenty i její vlastní CSS styl, připrav si v něm třídy, které komponentu adekvátně nastylují, a aplikuj na `<div>` osoby tu správnou třídu podle pohlaví.

