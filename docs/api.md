# API

Il progetto **Mini-Blog** utilizza le API gratuite di
[JSONPlaceholder](https://jsonplaceholder.typicode.com/) per popolare le pagine
con dati fittizi. Tutte le richieste sono di sola lettura (`GET`) e vengono
effettuate via `fetch` dal file [script.js](../script.js).

## URL di base

```
https://jsonplaceholder.typicode.com
```

## Endpoint utilizzati

### Post

```
GET https://jsonplaceholder.typicode.com/posts
```

- **Usato da:** `posts.html`
- **Descrizione:** restituisce l'elenco dei post. Nel sito vengono mostrati solo
  i primi 12.
- **Esempio di risposta (singolo elemento):**

```json
{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident...",
  "body": "quia et suscipit suscipit recusandae..."
}
```

| Campo    | Tipo   | Descrizione             |
| -------- | ------ | ----------------------- |
| `userId` | number | ID dell'autore del post |
| `id`     | number | ID univoco del post     |
| `title`  | string | Titolo del post         |
| `body`   | string | Contenuto del post      |

### Utenti / Autori

```
GET https://jsonplaceholder.typicode.com/users
```

- **Usato da:** `autori.html` e `posts.html` (per associare ogni post al suo
  autore).
- **Descrizione:** restituisce l'elenco degli utenti. Nella pagina autori
  vengono mostrati solo i primi 10.
- **Esempio di risposta (singolo elemento):**

```json
{
  "id": 1,
  "name": "Leanne Graham",
  "email": "Sincere@april.biz",
  "address": {
    "city": "Gwenborough"
  },
  "company": {
    "name": "Romaguera-Crona"
  }
}
```

| Campo          | Tipo   | Descrizione            |
| -------------- | ------ | ---------------------- |
| `id`           | number | ID univoco dell'utente |
| `name`         | string | Nome dell'autore       |
| `email`        | string | Indirizzo email        |
| `address.city` | string | Città dell'autore      |
| `company.name` | string | Azienda dell'autore    |

## Come vengono usate le API

- Nella **pagina post** vengono richiesti in parallelo gli endpoint `/posts` e
  `/users`: ogni post viene poi abbinato al proprio autore tramite il campo
  `userId`.
- Nella **pagina autori** viene richiesto solo l'endpoint `/users`.
- I dati di testo provenienti dalle API vengono sempre ripuliti con una funzione
  di escape dell'HTML prima di essere inseriti nella pagina, per evitare
  problemi di sicurezza (XSS).

## Gestione degli errori

Se una richiesta non va a buon fine (es. assenza di connessione o servizio non
raggiungibile), il sito mostra un messaggio di avviso all'utente e l'errore HTTP
viene segnalato nella console del browser.

## Note

- JSONPlaceholder è un servizio di test: i dati sono fittizi e le eventuali
  operazioni di scrittura (`POST`, `PUT`, `DELETE`) vengono simulate ma **non**
  salvate realmente. Questo progetto usa solo richieste in lettura.
- Non è richiesta alcuna chiave di autenticazione (API key).
