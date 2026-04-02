# Cod reducere Notino — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Notino** de pe [shopilo.ro](https://shopilo.ro/magazin/notino.ro). Returneaza **cupoane Notino** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-notino](https://shopilo-ro.github.io/cod-reducere-notino/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-notino
cd cod-reducere-notino
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Notino",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% reducere la intreaga comanda",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/notino.ro"
  }
]
```

## Cupoane Notino disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 15% | 15% reducere la intreaga comanda | [shopilo.ro](https://shopilo.ro/magazin/notino.ro) |

Codurile active: **[shopilo.ro/magazin/notino.ro](https://shopilo.ro/magazin/notino.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Notino?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/notino.ro), adauga produsele in cos pe Notino, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Notino?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Notino?
Pagina [shopilo.ro/magazin/notino.ro](https://shopilo.ro/magazin/notino.ro) este actualizata zilnic cu cele mai noi cod reducere Notino, voucher Notino si cupon promotional Notino.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Notino

Notino este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/notino.ro) cele mai bune cod reducere Notino, cupoane Notino verificate si voucher Notino active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-notino
```

```javascript
const { fetchCoupons } = require('cod-reducere-notino');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
