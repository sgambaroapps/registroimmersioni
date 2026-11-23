# Pagina di presentazione di Nautilus - Registro Immersioni

Questa cartella è il sito di presentazione del programma per Windows
**Nautilus - Registro Immersioni**: il registro delle immersioni per diving
center e associazioni subacquee (legge 70/2026). È una pagina sola, in
italiano e in inglese, con il pulsante per scaricarlo dal Microsoft Store.
Ha la stessa grafica della pagina di Nautilus DiveKit.

Indirizzo:
**https://sgambaroapps.github.io/registroimmersioni/**

> L'informativa sulla privacy resta dove è
> (`https://sgambaroapps.github.io/nautilus-privacy/registro.html`, repository
> `nautilus-privacy`): quell'indirizzo è dichiarato al Microsoft Store e non va
> toccato. Questa pagina la richiama in fondo.

## Com'è fatta

- **Un file solo** (`index.html`) con tutte e due le lingue: la pagina mostra
  quella del browser (inglese se non è l'italiano) e si cambia con i pulsanti in
  alto a destra. Con `#it` o `#en` in fondo all'indirizzo si apre direttamente
  in quella lingua. Senza JavaScript si vedono le due lingue una sotto l'altra.
- `assets/icona.png` è l'icona del programma, `assets/divekit.png` quella di
  Nautilus DiveKit, `assets/og.jpg` l'immagine che compare quando il link viene
  mandato su WhatsApp o pubblicato su Facebook.
- `assets/shots/` contiene 5 schermate del programma (le stesse del Microsoft
  Store, con dati inventati), rimpicciolite per il web.
- `assets/badge/microsoft-it.svg` e `microsoft-en.svg` sono i badge ufficiali
  «Scarica da Microsoft» (generatore di Microsoft). Se mancano, al loro posto
  compare un pulsante bianco «Microsoft Store»: non si rompe niente.
- **Nessun tracciamento**: niente cookie, niente statistiche, nessuna chiamata a
  servizi esterni.

## Se vuoi cambiare i testi

La pagina è generata da uno script che tiene allineate le due lingue e prende
la grafica dalla pagina di Nautilus DiveKit:
`D:\APP Nautilus ALTRO\materiali-lancio\sorgenti\genera_sito_registro.py`.
Si modificano i testi là dentro (dizionario `T`) e si rilancia con
`py genera_sito_registro.py`: rifà `index.html` e le immagini.
