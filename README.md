# Sågenvägen – förslag (statisk sida)

Vanlig statisk HTML, inga beroenden, ingen byggprocess. Publiceras med GitHub Pages från rotmappen på `main`. Alla länkar och bildhänvisningar är relativa, så sidan fungerar under valfri sökväg, t.ex. `/sagenvagen-exempel/`.

## Filer (alla ligger i repots rot)
- `index.html` – kundpresentationen (startsida)
- `balkongen.html` (1a), `anslagstavlan.html` (1b), `omradet.html` (1c)
- `rorelse-dampad.html` (1e), `rorelse-uttrycksfull.html` (1d)
- `gard.jpg` – gården / husen (omslag, 1a, 1b)
- `balkonger.jpg` – balkonger i hösten (1a, 1b, 1c)
- `fasad.jpg` – fasad med balkonger (index, 1c)
- `dg-logo-black.png`, `dg-logo-white.png` – loggorna (PNG, genomskinlig bakgrund; svart för ljus bakgrund, vit för mörk)

Fotona är JPG, max ca 1800 px bredd. Det finns ingen `img/`-mapp och ingen `.htaccess`. Filnamn är skiftlägeskänsliga på GitHub Pages.

## Att tänka på
1. Endast nåbar med länk: repot är publikt och sidorna har `<meta name="robots" content="noindex, nofollow, noarchive">`. Behåll den i varje sida. Lägg INTE repots adress i någon `robots.txt`: den filen är offentlig och skulle avslöja adressen. Det är inte åtkomstskydd: den som har länken kan öppna sidan.
2. Typsnitt: sidorna hämtar Google Fonts (Familjen Grotesk, Hanken Grotesk, Caveat, Instrument Serif) från Google. Ladda hellre ned och servera dem själva (GDPR).
3. Alla sidor är anpassade för mobil (brytpunkt 820 px) och testade i 390 px och 1280 px bredd. Testa gärna på riktig telefon.
4. Alla texter, nyheter och tider är exempeltext.
