# Codice sconto Sorgenia, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Sorgenia** da [shopilo.it](https://shopilo.it/negozi/sorgenia.it). Restituisce **coupon Sorgenia** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-sorgenia](https://shopilo-it.github.io/codice-sconto-sorgenia/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-sorgenia
cd codice-sconto-sorgenia
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Sorgenia",
    "code": "SHOPILO30",
    "discount": "30 EUR",
    "description": "30 EUR di sconto sulla prima bolletta energia",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/sorgenia.it"
  }
]
```

## Coupon Sorgenia disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 30 EUR | 30 EUR di sconto sulla prima bolletta energia | [shopilo.it](https://shopilo.it/negozi/sorgenia.it) |

Codici attivi: **[shopilo.it/negozi/sorgenia.it](https://shopilo.it/negozi/sorgenia.it)**

## Domande frequenti

### Come utilizzo un codice sconto Sorgenia?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/sorgenia.it), aggiungi i prodotti al carrello su Sorgenia e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Sorgenia?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Sorgenia piu recenti?
La pagina [shopilo.it/negozi/sorgenia.it](https://shopilo.it/negozi/sorgenia.it) viene aggiornata quotidianamente con i codici sconto Sorgenia, voucher Sorgenia e coupon promozionali Sorgenia piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Sorgenia

Sorgenia e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/sorgenia.it) trovi i migliori codici sconto Sorgenia, coupon Sorgenia verificati e voucher Sorgenia attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-sorgenia
```

```javascript
const { fetchCoupons } = require('codice-sconto-sorgenia');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
