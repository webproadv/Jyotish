# Jyotish Vedanga — sito di studio

Sito statico (HTML puro, nessuna build necessaria) con gli schemi e gli strumenti di studio per il corso di Jyotish Vedanga.

## Struttura

- `index.html` — pagina principale con i link a tutti gli strumenti
- `schemi/segni-case.html` — tabella Segni e Case
- `schemi/dignita-planetarie.html` — infografica Dignità Planetarie
- `schemi/costellazione-dignita.html` — grafo interattivo delle dignità
- `schemi/ruota-dignita.html` — ruota zodiacale a 7 anelli
- `assets/Percorso_Studio_Jyotish.pdf` / `.docx` — percorso di studio in 9 settimane

## Come pubblicarlo su GitHub

Dalla cartella estratta dallo zip:

```bash
git init
git add .
git commit -m "Sito Jyotish Vedanga: schemi e percorso di studio"
git branch -M main
git remote add origin https://github.com/webproadv/Jyotish.git
git push -u origin main
```

Se il repository su GitHub contiene già dei file (es. un README creato dall'interfaccia), puoi invece clonarlo prima e copiarci dentro il contenuto di questo zip:

```bash
git clone https://github.com/webproadv/Jyotish.git
cp -r jyotish-site/* Jyotish/
cd Jyotish
git add .
git commit -m "Sito Jyotish Vedanga: schemi e percorso di studio"
git push
```

## Deploy su Vercel

Una volta che il contenuto è su GitHub, il progetto Vercel verrà collegato al repository `webproadv/Jyotish` e pubblicato all'indirizzo `jyotish.vercel.app`. Non è necessaria nessuna configurazione di build: è un sito statico, Vercel lo riconosce automaticamente.

## Aggiornamenti futuri

Ogni nuovo schema o strumento verrà aggiunto a questa stessa struttura (nuova pagina dentro `schemi/`, più un nuovo link nella `index.html`) e, una volta inviato su GitHub, sarà pubblicato automaticamente su `jyotish.vercel.app` ad ogni push sul branch `main`.
