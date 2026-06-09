# Installazione Repo

Per installare il progetto è necessario avere installato git.

## Requisiti

- Un browser moderno (Chrome, Firefox, Edge, Safari...)
- Connessione a Internet (per Bootstrap via CDN e per le API esterne)
- [Git](https://git-scm.com/) oppure la [GitHub CLI (`gh`)](https://cli.github.com/) per clonare la repository

## Passaggi

- Aprire il terminale

- Verificare che git sia installato:

  ```bash
  git --version
  ```

  Se il comando restituisce un numero di versione, git è installato
  correttamente. In caso contrario, installalo da
  [git-scm.com](https://git-scm.com/).

- Clonare la repository:

  ```bash
  git clone https://github.com/halocavo92/esame_doc.git
  ```

  In alternativa, con la GitHub CLI:

  ```bash
  gh repo clone halocavo92/esame_doc
  ```

- Entrare nella cartella del progetto:

  ```bash
  cd esame_doc
  ```

## Avvio del sito

Trattandosi di un sito statico, non è necessario alcun server o installazione di
dipendenze. È sufficiente aprire il file `index.html` in un browser:

- fare doppio clic sul file `index.html`, oppure

- aprirlo dal terminale:

  ```bash
  # Linux
  xdg-open index.html

  # macOS
  open index.html

  # Windows
  start index.html
  ```

> **Nota:** è necessaria una connessione a Internet attiva, perché il sito
> carica Bootstrap da CDN e i dati dei post e degli autori dalle API di
> JSONPlaceholder.

## Versione online

Il sito è già pubblicato tramite GitHub Pages ed è raggiungibile senza alcuna
installazione al seguente indirizzo:

https://halocavo92.github.io/esame_doc/

## Documentazione correlata

- [Domande frequenti (FAQ)](faq.md)
- [API utilizzate](api.md)
