<p align="center">
  <img src="assets/cover.svg" alt="Prompt Search — ricerca locale per archivi di prompt" width="100%">
</p>

# Prompt Search.

**Avevo centinaia di prompt. Il problema non era conservarli: era ritrovarli quando servivano davvero.**

Nel tempo il mio archivio era diventato una struttura di cartelle, sottocartelle e file Markdown. Ordinata, sì. Ma ogni volta che cercavo qualcosa dovevo ricordare dove fosse, aprire la cartella giusta, trovare il file, controllarlo e copiarlo.

Troppi passaggi per una cosa che dovrebbe richiedere pochi secondi.

Da qui nasce **Prompt Search**.

Non volevo costruire un gestionale, un database o un altro servizio online. Volevo una cosa molto più semplice:

> **apro una pagina → scrivo una parola → trovo il prompt → lo copio**

## Da archivio a ricerca immediata

<p align="center">
  <img src="assets/archive-to-search.svg" alt="Da cartelle Markdown a una ricerca immediata" width="100%">
</p>

Prompt Search trasforma un archivio di file Markdown in una **pagina HTML locale e portatile**.

Nella mia build privata l'archivio contiene **572 prompt**, con una selezione principale di **222** elementi. Questi contenuti **non sono presenti in questa repository pubblica**.

La logica del progetto è invece tutta qui:

**CERCA → APRI → COPIA → USA**

## Cosa fa

- ricerca nei titoli e nei contenuti;
- vista principale e archivio completo;
- navigazione per categorie;
- apertura del contenuto in una pagina leggibile;
- copia negli appunti con un clic;
- download del singolo elemento come `.md`;
- Preferiti e Cestino salvati nel browser;
- export dei Preferiti;
- backup dell'HTML;
- utilizzo offline.

<p align="center">
  <img src="assets/prompt-detail.svg" alt="Vista di dettaglio di Prompt Search" width="100%">
</p>

## Perché un solo file HTML

Per me era importante che lo strumento restasse semplice.

`PROMPT_SEARCH.html` contiene interfaccia, CSS e JavaScript. Non richiede:

- backend;
- database;
- API;
- framework;
- account;
- installazione.

Scarichi il file, lo apri nel browser e funziona.

Su Mac, `WIDGET_APRI_RICERCA.html` può essere usato come piccolo launcher tramite un alias sulla Scrivania o nel Dock.

## Avvio

Clona o scarica la repository e apri:

```text
PROMPT_SEARCH.html
```

La build pubblica parte volutamente **vuota**.

## Perché non ci sono prompt nella repository

Questa è una scelta precisa.

I prompt che uso nel mio lavoro sono contenuti personali e professionali. Volevo raccontare e condividere **il sistema che ho costruito**, non pubblicare il mio archivio.

Per questo la versione pubblica contiene:

- il codice;
- l'interfaccia;
- il motore di ricerca;
- le funzioni locali;
- gli asset grafici;
- **zero prompt del mio archivio privato**.

Nel file pubblico, `prompt-data` è intenzionalmente vuoto.

La repository privata e quella pubblica hanno inoltre **cronologie Git separate**, per evitare che vecchi commit possano esporre contenuti rimossi.

## Una precisazione tecnica

Prompt Search è uno **snapshot dell'archivio**, non un file manager.

Non osserva automaticamente una cartella del computer e non modifica i file Markdown originali. I dati devono essere incorporati nell'HTML quando si genera la propria build.

Preferiti e Cestino vengono gestiti localmente nel browser; le funzioni di salvataggio e backup permettono di conservarne lo stato.

## Struttura

```text
prompt-search/
├── PROMPT_SEARCH.html
├── WIDGET_APRI_RICERCA.html
├── README.md
├── PUBLIC_BUILD.md
├── .gitignore
└── assets/
    ├── cover.svg
    ├── archive-to-search.svg
    └── prompt-detail.svg
```

## Privacy

La build pubblica non contiene il mio archivio personale, non richiede account e non usa API esterne per funzionare.

---

Made with ♥ in Milan by **Emanuele BDC**
