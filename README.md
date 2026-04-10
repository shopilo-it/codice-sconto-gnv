# Codice sconto GNV, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto GNV** da [shopilo.it](https://shopilo.it/negozi/gnv.it). Restituisce **coupon GNV** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-gnv](https://shopilo-it.github.io/codice-sconto-gnv/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-gnv
cd codice-sconto-gnv
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "GNV",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su traghetti per Sardegna e Sicilia",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/gnv.it"
  }
]
```

## Coupon GNV disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su traghetti per Sardegna e Sicilia | [shopilo.it](https://shopilo.it/negozi/gnv.it) |

Codici attivi: **[shopilo.it/negozi/gnv.it](https://shopilo.it/negozi/gnv.it)**

## Domande frequenti

### Come utilizzo un codice sconto GNV?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/gnv.it), aggiungi i prodotti al carrello su GNV e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon GNV?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher GNV piu recenti?
La pagina [shopilo.it/negozi/gnv.it](https://shopilo.it/negozi/gnv.it) viene aggiornata quotidianamente con i codici sconto GNV, voucher GNV e coupon promozionali GNV piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su GNV

GNV e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/gnv.it) trovi i migliori codici sconto GNV, coupon GNV verificati e voucher GNV attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-gnv
```

```javascript
const { fetchCoupons } = require('codice-sconto-gnv');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
