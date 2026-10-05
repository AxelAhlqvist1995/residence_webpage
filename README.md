# Föreningens hemsida

Statisk hemsida för Brf Pilen 32 (https://brfpilen32.se) – information till köpare och mäklare.
Ingen databas, inget CMS, inget att säkerhetsuppdatera.

## Filer

- `index.html` – hela hemsidan (en sida). All text redigeras här.
- `dokument/` – PDF:er (årsredovisningar, stadgar, ordningsregler, energideklaration).
- `bilder/` – foton. `gard-1.jpg` är toppbilden.
- `CNAME` – domännamnet (brfpilen32.se). Ändra inte.

## Uppdatera innehåll (ca en gång per år)

1. Gå till repot på GitHub och öppna `index.html`.
2. Klicka på pennan (Edit), ändra texten mellan taggarna, t.ex. `<td>1 234 kr</td>`.
3. Uppdatera "Senast uppdaterad" längst ner.
4. Klicka **Commit changes**. Sidan publiceras automatiskt inom någon minut.

Ny årsredovisning: gå in i mappen `dokument/` → **Add file → Upload files**,
döp filen till t.ex. `arsredovisning-2026.pdf` och lägg till en rad i listan
under "Årsredovisningar" i `index.html`. Ta gärna bort den äldsta.

Filnamn: små bokstäver, inga mellanslag och inga å/ä/ö.

## Publicering

Hostas gratis på GitHub Pages (eller Cloudflare Pages) direkt från grenen `main`.

**GitHub Pages:** Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)`.
Under *Custom domain*, ange `brfpilen32.se` och kryssa i *Enforce HTTPS*.

**DNS hos Loopia** (customerzone.loopia.com → brfpilen32.se → DNS-editor):

| Typ   | Namn  | Värde                         |
|-------|-------|-------------------------------|
| A     | @     | 185.199.108.153               |
| A     | @     | 185.199.109.153               |
| A     | @     | 185.199.110.153               |
| A     | @     | 185.199.111.153               |
| CNAME | www   | AxelAhlqvist1995.github.io    |

## Ansvar och åtkomst

- Domänen ska vara registrerad på föreningens organisationsnummer, med föreningens
  gemensamma e-post som kontoadress.
- Minst två personer i styrelsen ska ha åtkomst till både domänkontot och GitHub-repot.
- Publicera inga medlemsnamn, lägenhetsnummer kopplade till personer eller privata
  telefonnummer.
