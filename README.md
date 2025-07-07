# BKeep – Glavni Repozitorij

Dobrodošli v glavnem repozitoriju za projekt **BKeep**, ki združuje vse module aplikacije:

- `bkeep-api` – Backend storitev (API)
- `bkeep-web-app` – Web frontend
- `bkeep-scraper` – Scraperji podatkov
- `bkeep-prevajanje` – Domensko specifični programski jezik

---

## Namestitev (kloniranje s submoduli)

### 1. Kloniraj repozitorij s submoduli:

```bash
git clone --recurse-submodules git@github.com:BKeepTM/BKeep.git
cd BKeep
```
### 2. Posodobi submodule na zadnje verzije:
```bash
git submodule update --remote --merge
```
