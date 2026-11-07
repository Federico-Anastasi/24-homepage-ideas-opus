# 24 home page

Ventiquattro prime pagine diverse per lo stesso contenuto: un titolo e quattro progetti. Sono state disegnate da Claude Opus 5.5
per il sito di Federico Anastasi; qui sono ripulite e neutre, pronte da prendere e adattare al tuo progetto. Licenza MIT.

Ogni pagina è un solo file HTML (CSS e JavaScript dentro, nessun passaggio di compilazione), pensato per il telefono in verticale.

## Come si usano

1. Apri `index.html` da un server locale (vedi sotto): vedi le 24 pagine dentro un telefono, con numero, nome e link per aprirle.
2. Scegli quella che ti piace e copia il suo file da `template/` nel tuo progetto, insieme alla cartella `risorse/`
   (i percorsi sono relativi: `template/` e `risorse/` devono restare vicine, oppure aggiorna i percorsi `../risorse/`).
3. Apri il file: in cima c'è un commento «COME USARLA» che dice dove stanno il titolo, i progetti e le icone in quella pagina.
4. Sostituisci:
   - il titolo: «Il tuo spazio aperto» e «di Nome Cognome»;
   - i quattro progetti: «Progetto uno … quattro», la frase «una frase breve» e la categoria;
   - le icone: `risorse/progetto-1.svg … progetto-4.svg` (quadrate, sfondo trasparente: puoi tenere gli stessi nomi);
   - i link `#progetto-1 … #progetto-4`, con gli indirizzi dei tuoi progetti.

In alcune pagine il testo non sta solo nell'HTML ma anche nello script, perché è disegnato su un canvas o su una texture 3D
(12, 16, 18, 19, 20, 23) o scritto da una demo animata (17): il commento in cima al file dice dove.

### Server locale

Le pagine con grafica 3D caricano le immagini dentro WebGL e non funzionano aprendole con un doppio clic (`file://`).
Basta un server qualunque, dalla cartella del repo:

```
python -m http.server 8000
```

poi apri `http://127.0.0.1:8000/`.

## Librerie e risorse esterne

Servono internet al primo caricamento.

- **Caratteri**: tutte le pagine usano un carattere da Google Fonts (con un ripiego di sistema se non si carica).
- **three.js r128** da cdnjs: `12-titolo-cromato`, `21-oggetti`, `22-diorama`, `23-particelle`, `24-acrilico`.
- Le altre pagine non usano librerie: solo CSS, SVG, canvas 2D o WebGL scritto a mano (`05-aurora`, `09-cromo-liquido`, `15-vetro-acidato`).

Per usarle offline scarica i caratteri e `three.min.js` e cambia gli indirizzi nei file.

## Le 24 pagine

| n. | nome | idea |
|----|------|------|
| 01 | manifesto | impaginazione svizzera, titolo enorme, filetto rosso che si disegna |
| 02 | risograph | stampa a tre inchiostri, forme sovrapposte e fuori registro |
| 03 | bauhaus | forme piatte e colori primari |
| 04 | carta | carta tagliata a strati, con ombre di spessore |
| 05 | aurora | gradiente caldo che scorre, in WebGL |
| 06 | grana calda | bande di luce con grana di pellicola |
| 07 | liquido | quattro gocce che si fondono e si separano |
| 08 | campo | quattro poli che si spostano col dito |
| 09 | cromo liquido | gocce di cromo con riflesso che segue il dito |
| 10 | alluminio | targhe di alluminio spazzolato |
| 11 | ottone | targhette smaltate in ottone |
| 12 | titolo cromato | titolo 3D cromato e quattro gettoni (three.js) |
| 13 | insegne | insegne al neon su un muro di mattoni |
| 14 | olografico | bollini olografici in rilievo |
| 15 | vetro acidato | lastre di vetro acidato |
| 16 | oscilloscopio | figure di Lissajous a fosforo ambra |
| 17 | terminale | un terminale con quattro processi vivi |
| 18 | led | pannello a matrice di LED |
| 19 | solari | tabellone a palette girevoli, come in stazione |
| 20 | televideo | pagina di teletext con vetro di televisore |
| 21 | oggetti | quattro oggetti 3D lucidi (three.js) |
| 22 | diorama | stanzetta isometrica 3D (three.js) |
| 23 | particelle | trentamila punti di luce che compongono il titolo (three.js) |
| 24 | acrilico | lastre di acrilico che catturano la luce (three.js) |

## Licenza

MIT, vedi `LICENSE`.

## English

24 different home pages for the same content: a title and four projects, designed by Claude Opus 5.5 for Federico Anastasi's website,
cleaned up and neutral so you can take one and make it yours. Each page is a single HTML file; open `index.html` through any static
server (for example `python -m http.server`) to browse them, copy the one you like together with `risorse/`, and replace the title,
the four projects and the icons (a comment at the top of each file says where). Five pages use three.js from a CDN; all pages load
a font from Google Fonts. MIT licensed.
