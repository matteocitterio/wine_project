# wine_project

Il dataset può essere scaricato al link: https://www.dropbox.com/s/pnsghv18r7h4mi6/wine_challenge.csv?dl=0

si tratta di un csv, in python per lavorarci è sufficiente: `df=pd.read_csv('path', index_col=0)`

i dati sono stati scaricati da vivino (https://www.vivino.com), una piattaforma online di compra-vendita di vini.

## contenuto:

-) `Sku`: gli oggetti sono indicizzati a partire dallo sku, una stringa univoca per ogni vino (nome del vino + cantina + annata + formato bottiglia)
-) `Wine`: nome del vino
-) `Winery`: nome della cantina
-) `Year`: Annata della bottiglia. Alcuni vini sono cuvee, ovvero sono un blend di diverse annate. Per questi si usa la terminologia `N.V.`, non-vintage
-) `Style`: alcuni vini sono catalogati in base alo stile che può essere un metodo produttivo, le uve utilizzate o la regione di provenienza. Troverete, ad esempio, `barolo italiano` o `Pinot Noir Alsaziano` e così via.
-) `Region`: Regione di provenienza, ad esempio `Piemonte` o `Champagne`.
-) `Country`: Il paese di provenienza, ad esempio `Italia` o `Francia`
-) `Volume [ml]`: il formato della bottiglia. Il più comune è 750 ml ma esistono anche le magnum da 1500 ml e altri formati.

Le quantità che possono variare su base giornaliera sono:

`Price`: il prezzo al dato giorno del vino in EURO
`Rating`: vivino permette agni utenti della piattaforma di valutare il vino su una scala da 1.0 a 5.0 con intervalli decimali. il rating mostrato è la media per una certa annata del vino considerato sulle valutazioni degli utenti
`num_review`: Numero delle recensioni ricevute da una certa bottiglia
`Date`: data in cui sono state scaricate le informazioni che variano nel tempo
