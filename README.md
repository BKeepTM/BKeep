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
<br>

# Komponente platforme BKeep
## Spletna aplikacija

Spletni vmesnik je namenjen upravljanju čebelarskih podatkov preko brskalnika. Omogoča pregled in upravljanje čebelnjakov, panjev, meritev, zapiskov ter drugih podatkov, zbranih preko mobilne aplikacije in IoT naprav.

Uporabnikom omogoča centraliziran pregled nad stanjem sistema, pregled statističnih podatkov, analizo zdravja in števila populacije panja s pomočjo računalniškega vida ter povezovanje z ostalimi moduli platforme BKeep.

<img width="2530" height="1326" alt="image" src="https://github.com/user-attachments/assets/02043756-05be-427a-bbf7-844ea7ff12cf" /> <br>
<img width="2528" height="626" alt="image" src="https://github.com/user-attachments/assets/33e290e9-c5d6-4ae6-9393-8370d1446b82" /> <br>

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
Glavna funkcijonalost namizne aplikacije je interaktivni zemljevid, ki prikazuje stanje in lokacije panjev. Podpira vse osnovne funkcionalnosti Bkeep (kot android in spletna rešitev). Aplikacija je povezana s scraperjem, ki prejema podatke o trenutnem vremenu in jih prikaže ter po želji upošteva pri simulaciji pridelka.

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/6623f814-a182-48fd-a636-6e63fa8fd7ae" />

## IoT naprave

Tehnica za merjenje mase panjev je zgrajena iz 4 merilnih celic, ki so povezane na HX71. Ta pretvori analogno meritev v digitalni signal (sprememba mase) in ga posreduje mikrokrmilniku (ESP32), kjer se z ustrezno kalibracijo pretvori v meritev mase. Ta mertiev se preko APIja pošlje in shrani v podatkovno bazo ter prikaže v uporabniškem vmesniku (npr. spletni strani, android aplikaciji). <br>

<img width="4000" height="1800" alt="20260202_160606" src="https://github.com/user-attachments/assets/ed9b8932-a86a-441b-9326-516018d64fda" />


