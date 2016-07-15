
## Srpski prevod za Alfresco
----------

Dvojezični prevod Alfresco Community verzije na srpsko latinično i ćirilično pismo. Prevedeni su svi bitni delovi Share korisničkog interfejsa, kao i poruke Alfresco repozitorijuma (model podataka, sistemske poruke, akcije, radni tokovi, web sckripte itd.)

**Uputstvo za instalaciju:**

1. Zaustaviti Alfresco server
2. Kopirati **jar** fajl na putanju:

	```
	*alfresco instalacija*/tomcat/shared/lib/
	```
3. Podesiti željeni jezik (srpsku latinicu ili ćirilicu) kao podrazumevani u pregledaču koji se koristi za pristup Alfresco-u.
4. Startovati Alfresco.

> ***Napomena:*** Pošto je teško utvrditi *Locale* oznake koje će biti prihvaćene u svim pretraživačima, mi smo odlučili da koristimo oznaku **[sr]** za latinicu i **[sx]** za ćirilicu. sx nije zvanični previks za srpsko ćirilično pismo, ali mi smo usvojili tu formu jer je kratko, a većina pretraživača ionako nema ćirilično pismo u izboru jezika.

**Podešavanje internet pretraživača:**

 1. **Mozilla Firefox**
	 * Ukucajte u adresni prostor tekst *about:config* i pritisnite enter. Ova akcija bi trebalo da u glavnom prozoru prikaže stranicu sa svim internim paramtetrima pretraživača. Ukoliko prvi put otvarate ovu stranicu pre njenog otvaranja biće prikazana stranica sa upozorenjem, na kojoj je potrebno kliknuti na dugme *I'll be careful.*
	 * Pronaći parametar sa nazivom "**intl.accept_languages**" (ukucati taj naziv u polje za pretragu ukoliko je potrebno).
	 * Dvaput kliknuti na parametar, čime se otvara dijalog za ručni unos. Dodati na početak postojeće vrednosti "**sr**" za latinicu ili "**sx**" za ćirilicu. (Ukoliko posle novo unete vrednosti stoji još neka, obavezno je odvojiti karakterom zareza "**,**", npr: "*sr,en-us,en*").
	 * Kliknuti na dugme Ok i pristupiti Share stranici.
	> ***Alternativno.*** Firefox  zvanično podržava Srpsku latinicu, pa ukoliko želimo to pismo postoji jednostavniji postupak za podešavanje. Otvoriti Options, odabrati Content, kliknuti na dugme Choose.. u sekciji Languages, zatim naći u listi jezika *Serbian [sr]* i kliknuti na dugme Add (Ukoliko imamo više jezika u listi, pomeriti Serbian na početak liste). Pošto u postojećem spisku nema Ćirilice, gore je opisan jedinstveni postupak za oba pisma.
	
 3. **Google Chrome**
	 * Potrebno je u editoru teksta otvoriti konfiguracioni fajl Chrome-a. Taj fajl se uobičajeno nalazi na putanji:
	```
	%USER HOME%\AppData\Local\Google\Chrome\User Data\Default\Preferences
	```
	* U tom fajlu naći parametar sa nazivom "**accept_languages**". U zavisnosti od toga koji jezik želite dodajte na početak vrednosti tog parametra "**sr**" za latinicu ili "**sx**" za ćirilicu. Primer:
	
		```
		{"accept_languages":"sr,en-US,en"}
		```
	* Zatvoriti i ponovo pokrenuti Chrome pretraživač, nakon čega možete pristupiti Share stranici.
	
	> ***Alternativa.*** Slično kao i kod Firefox-a i Chrome ima lakši postupak za podešavanje Srpske latinice. Otvoriti Podešavanja, skroz na dnu stranice kliknuti na Prikaži Napredna Podešavanja, u sekciji Jezici kliknuti na dugme Podešavanje Jezika i Unosa. Kliknuti na dugme Add i u listi jezika pronaći *Serbian - Српски*. Kliknuti na Ok i prevući mišem srpski na početak liste dodatih jezika. Nakon ovoga možemo pristupiti Share stranici. Ako korisnik odabere da Chrome bude prikazan na ovom *Serbian - Српски* jeziku, on će biti prikazan na ćiriličnom pismu, ali i pored toga Share će biti prikazan na latiničnom. Nažalost zvanično Google ne nudi opciju za zasebnim odabiranjem ova dva pisma.


 4. **Microsoft Internet Explorer**
	* Otvoriti Internet Options. Na stranici General, Sekcija Appearance kliknuti na dugme Languages, pa na dugme Add.
	* Za podešavanje latinice naći u listi jezika *Serbian (Latin) [sr-Latin]*. Za podešavanje ćirilice, potrebno je uneti vrednost "**sx**" u polje User Defined. Kliknuti Ok.
	* Upravo dodati jezik premestiti na početak liste jezika (dugmetom Move Up). Kliknuti Ok i pristupiti Share stranici.

## Serbian dual language pack for Alfresco
----------

Here you can find translation of Alfresco Community version on Serbian language. Translated files are available in two versions, one for Serbian Cyrillic alphabet and other for Serbian Latin alphabet. Share interface is completely translated alongside repository internal messages (data model, workflows and actions, system messages etc.).

**Installation instructions:**

1. Stop Alfresco server
2. Copy the downloaded **jar** file in the following location:

	```
	*alfresco installation*/tomcat/shared/lib/
	```
3. Set the default language on the internet browser that is used to access Alfresco to either Serbian Latin or Serbian Cyrillic.
4. Start Alfresco.

> ***Note:*** Since there is no standard for Locales that will be accepted across all browsers, we decided to use **[sr]** as a mark for Serbian latin alphabet and **[sx]** for cyrillic. For example official Java supported locale for cyrillic is sr_RS  (sr_Latn_RS for latin) but this is already widely used as extension for latin locale. Similarly sx_RS used to be specified for cyrillic locale in web applications, therefore we decided to shorten this extensions to just sr and sx.

**Internet browser configuration:**

 1. **Mozilla Firefox**
	 * In the address bar type in *about:config* and press enter. This action should open up page with all the browsers internal settings. If you open this page for the first time, before it is opened a warning page will be shown, on which you should click button  *I'll be careful.*
	 * Find the property named "**intl.accept_languages**" (type this name in the search field if you have trouble finding it).
	 * Double click this property which opens dialog for manual entry. At the beginning of the field add text "**sr**" for latin or "**sx**" for cyrillic alphabet. (If this property already has some value, be sure to separate it from newly entered text by using comma "**,**", e.g.: "*sr,en-us,en*").
	 * Click the Ok button and access the Alfresco Share page.
	> ***Alternative.*** Firefox  officially supports Serbian latin alphabet, so if that's the language you want to set up there is an easier procedure. Open Options from Firefox menu, on the left side choose Content , than in section Languages click on the button Choose... On the opened dialog, in the list of languages, find the *Serbian [sr]* and click the Add button (if after this addition we have multiple languages in the list, move the Serbian to the top of the list). Cyrillic alphabet cannot be configured using this method.
	
 3. **Google Chrome**
	 * Open Chromes configuration file in any text editor. The usual location of this file is:
	```
	%USER HOME%\AppData\Local\Google\Chrome\User Data\Default\Preferences
	```
	* In this file find the parameter named "**accept_languages**". Depending on which language locale you want, add to the beginning of this parameter "**sr**" for latin or "**sx**"for cyrillic. For example:
	
		```
		{"accept_languages":"sr,en-US,en"}
		```
	* Restart the Chrome application, after which you can access Alfresco Share.
	
	> ***Alternative*** Similarly to Firefox, there is also easier and more intuitive method for configuring Serbian Latin locale. Open Settings, all the way at the bottom of Settings page click on Show advanced settings... then in the Languages section click on the button Language and input settings... Click the Add button and in the language list find *Serbian - Српски*. Click Ok, and move Serbian language to the beginning of the list by dragging it with the mouse. After this you can access Alfresco Share. If the user chooses to display Chrome in this *Serbian - Српски* language, Chrome interface will be translated to Serbian cyrillic, but regardless, Alfresco Share will be shown in latin alphabet. Unfortunately Chrome doesn't support two locales for one language.


 4. **Microsoft Internet Explorer**
	* Open Internet Options. On the General tab, section Appearance, click on the button Languages, then button Add.
	* To configure latin translation in the list of languages find *Serbian (Latin) [sr-Latin]*. For cyrillic translation, type in "**sx**" in the field User Defined. Click Ok.
	* Move the newly added language to the beginning of the list (by using the Move Up button). Click Ok and access Alfresco Share.


