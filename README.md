# Formato accettato per l'invio dei comunicati via email

Di seguito le regole e i tag speciali (shortcode) che è possibile usare per inviare un comunicato stampa tramite email.  
Questa formattazione è compatibile con il sistema integrato e consente la corretta creazione automatica del post sul sito.

---

## 📨 Oggetto della mail

**Formato richiesto**:  
`[Categoria] Titolo del comunicato`

- Il nome della categoria va racchiuso tra parentesi quadre `[ ]`
- La categoria **deve esistere già** nel sito (non viene creata automaticamente)
- Il resto dell'oggetto sarà il titolo visibile del post

**Esempio**:  
`[Eventi] Beauty Week Milano 2025`

---

## 📄 Corpo della mail

Il contenuto del comunicato deve essere compreso tra i tag `[start]` e `[end]`.  
Tutto ciò che si trova fuori da questi due tag **non verrà incluso** nel post.

### Struttura base consigliata

```
[start]
[title]Titolo SEO del comunicato[/title]
[desc]Breve descrizione ottimizzata per i motori di ricerca.[/desc]
[credits]Nome fotografo o fonte immagini[/credits]
tags: termine1, termine2,
date: 12 May, 2025

Testo del comunicato stampa vero e proprio, eventualmente con paragrafi, grassetti e link.

[end]
```

### 🏷 Campi speciali supportati

| Shortcode        | Descrizione                                              | Obbligatorio |
|------------------|----------------------------------------------------------|--------------|
| `[start]`        | Inizio del corpo del comunicato                          | ✅           |
| `[end]`          | Fine del corpo del comunicato                            | ✅           |
| `[title]...[/title]` | Titolo SEO (non mostrato nel contenuto)             | ❌           |
| `[desc]...[/desc]`   | Meta Description (non mostrato nel contenuto)           | ❌           |
| `[credits]...[/credits]` | Credito fotografico da associare al contenuto | ❌ |
| `tags:` seguito da parole chiave separate da virgola (minuscole) | Tag del post | ❌           |
| `date:` nel formato `22 Apr, 2025` | Data del comunicato (usata come data del post) | ❌  |

---

## 📎 Altri contenuti supportati

### 📷 Immagini

- È possibile **allegare immagini** all'email, ad esempio dopo averle scaricate da archivi online o servizi come WeTransfer.
- La **prima immagine** allegata verrà impostata come **immagine in evidenza** del post.

### 📄 PDF del comunicato

- È possibile specificare se il **PDF originale** del comunicato stampa debba essere incluso nel post.
- In tal caso, verrà salvato come file scaricabile e linkato automaticamente all'interno del contenuto.

---

## ✅ Esempio completo

```
Oggetto: [Eventi] Beauty Innovation Day Roma

[start]
[title]Beauty Innovation Day: innovazione e sostenibilità[/title]
[desc]Evento nazionale dedicato alle novità del settore estetico e del wellness.[/desc]
[credits]Fotografo: Maria Rossi[/credits]
tags: eventi, roma, beauty, innovazione
date: 14 May, 2025

Beauty Innovation Day si terrà a Roma il 14 maggio 2025 presso il centro congressi "La Nuvola".
Un appuntamento imperdibile per professionisti e aziende del settore.

[end]
```

---

## ❗️Note importanti

- I tag **devono essere scritti esattamente come indicato**, con parentesi quadre e senza spazi.
- I contenuti fuori da `[start]` e `[end]` **non saranno importati**.
- Se `[title]` o `[desc]` mancano, il post verrà comunque creato ma senza metadati SEO personalizzati.
