# BKeep – Glavni Repozitorij

Dobrodošli v glavnem repozitoriju za projekt **BKeep**, ki združuje vse module aplikacije:

- `bkeep-api` – Backend storitev (API)
- `bkeep-web-app` – Web frontend
- `bkeep-scraper` – Scraperji podatkov
- `bkeep-prevajanje` – Domensko specifični programski jezik
- `bkeep-pora` – Android platformna aplikacija
- `bkeep-rri` – Namizna aplikacija z interaktivnim zemljevidom
- `bkeep-blockchain` – Veriženje blokov podatkov panjev
- `ESP32` – Koda za ESP32 mikrokontroler

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

# Funkcionalnosti
## Spletna aplikacija

Spletni vmesnik je namenjen upravljanju čebelarskih podatkov preko brskalnika. Omogoča pregled in upravljanje čebelnjakov, panjev, meritev, zapiskov ter drugih podatkov, zbranih preko mobilne aplikacije in IoT naprav.

Uporabnikom omogoča centraliziran pregled nad stanjem sistema, analizo statističnih podatkov, analizo zdravja in števila populacije panja s pomočjo računalniškega vida ter povezovanje z ostalimi moduli platforme BKeep.

> Posnetek zaslona

## Mobilna aplikacija

Mobilna aplikacija je namenjena čebelarjem za delo na terenu in vključuje: <br> 
  - pregled čebelnjakov in panjev,
  - beleženje pregledov ter posegov,
  - vnos podatkov neposredno na lokaciji,
  - pregled lokacij na zemljevidu,
  - simuliranje pridelka medu na virtualnem panju glede na podane oz. izmerjene okoljske faktorje.
  - sinhronizacijo podatkov z ostalimi moduli sistema BKeep 

<img width="200" height="400" alt="image" src="https://github.com/user-attachments/assets/18f7fffd-5a44-4dc7-81b9-476cc438b2b9" />
<img width="200" height="400" alt="Posnetek zaslona 2026-07-08 150035" src="https://github.com/user-attachments/assets/bd665d69-fc61-477e-8ec6-750cb2f73d9a" />
<img width="200" height="400" alt="Posnetek zaslona 2026-07-08 150126" src="https://github.com/user-attachments/assets/b96c62a0-e4e1-4c99-acc7-d79d9ca6f6fe" />
<img width="200" height="400" alt="image" src="https://github.com/user-attachments/assets/7b74d150-5c69-4160-88db-b43d5e5f444b" />

## Namizna aplikacija
TODO


