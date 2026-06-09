# FAQ

Domande frequenti sul progetto **Mini-Blog**.

## Generale

### Che cos'è questo progetto?
È un mini-blog fittizio: un sito statico multipagina che utilizza le API di
[JSONPlaceholder](https://jsonplaceholder.typicode.com/) per popolare le pagine
con post e autori di esempio.

### Dove posso vedere il sito online?
Il sito è pubblicato tramite GitHub Pages al seguente link:
https://halocavo92.github.io/esame_doc/

### I dati mostrati sono reali?
No. Tutti i post e gli autori sono dati fittizzi forniti dalle API di
JSONPlaceholder, un servizio gratuito di test per sviluppatori.

## Installazione e utilizzo

### Come installo il progetto in locale?
Consulta la [Guida all'installazione](installazione.md). In sintesi, è
sufficiente clonare la repository e aprire il file `index.html` in un browser.

### Devo installare dipendenze o eseguire un server?
No. È un sito statico: Bootstrap viene caricato da CDN e i dati arrivano dalle
API esterne. Basta un browser moderno.

### Perché ho bisogno di una connessione a Internet?
La connessione serve per caricare Bootstrap (CSS e JS via CDN) e per scaricare i
dati dei post e degli autori dalle API di JSONPlaceholder.

## Funzionalità

### Quali pagine compongono il sito?
- **Homepage** (`index.html`): riassume lo scopo del sito
- **Post** (`posts.html`): mostra i post presi dalle API
- **Autori** (`autori.html`): mostra gli autori presi dalle API

### Il sito è ottimizzato per dispositivi mobili?
Sì. Il design è responsive grazie all'utilizzo di Bootstrap.

## Problemi comuni

### I post o gli autori non vengono visualizzati. Cosa faccio?
Verifica di essere connesso a Internet e che il servizio JSONPlaceholder sia
raggiungibile. Controlla inoltre la console del browser per eventuali errori.

### Lo stile della pagina non viene caricato.
Assicurati di avere una connessione attiva, dato che Bootstrap è caricato da CDN,
e che il file `style.css` sia presente nella cartella del progetto.

## Documentazione

- [Guida all'installazione](installazione.md)
- [API utilizzate](api.md)
