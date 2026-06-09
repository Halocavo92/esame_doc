# Mini-Blog
Questa repository serve per creare un mini-blog fittizio che utilizza le API di JSONplaceholder per popolare il sito con post e autori fittizzi.
Il progetto è un esempio di sito statico
il sito è visibile al seguente link :

https://halocavo92.github.io/esame_doc/



## Funzionalità

Il progetto include le seguenti funzionalità:

- Sito statico con multipagina
- Homepage che riassume il sito
- Pagina post che mostra i post presi dalle API esterne
- Pagina autori che mostra gli autori presi dalle API esterne
- Integra un design responsive anche per disp. mobili

## Tecnologie Utilizzate

- HTML
- CSS e Bootstrap(per design e responsive)
- JavaScript (per fetch dati dalle API esterne)
- API di JSONPlaceholder per i dati fittizzi

## Requisiti
- Un Browser Moderno
- Connessione a Internet (per Bootstrap e API esterne)
- Git o gh (per clonare la repository)

## API Utilizzate 

- Post https://jsonplaceholder.typicode.com/posts Pagina posts.html
- Utenti https://jsonplaceholder.typicode.com/users Pagina autori.html

## Struttura
Il progetto è strutturato in questo modo:

```
mini-blog-api/
├── README.md
├── index.html #homepage
├── posts.html #pagina post
├── autori.html #pagina autori
├── style.css #design responsive
├── script.js #fetch dati dalle API esterne
├── docs/ #documentazione
│ ├── installazione.md #come installare il progetto
│ ├── faq.md #domande frequenti
│ └── api.md # API esterne
├── data/ #dati fittizzi
└── assets/ 
└── immagini/
```

## Documentazione

La documentazione completa è disponibile nella cartella [`docs/`](docs/):

- [Guida all'installazione](docs/installazione.md) — come clonare e avviare il progetto
- [FAQ](docs/faq.md) — domande frequenti
- [API](docs/api.md) — dettaglio delle API esterne utilizzate

