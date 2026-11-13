# Sågenvägen – förslag (statisk sida)

Vanlig statisk HTML, inga beroenden, ingen byggprocess. Alla länkar är relativa, så mappen kan ligga under valfri sökväg, t.ex. `/exempel/sagenvagen-<slumpad-sträng>/`.

## Filer
- `index.html` – kundpresentationen (startsida)
- `balkongen.html` (1a), `anslagstavlan.html` (1b), `omradet.html` (1c)
- `rorelse-dampad.html` (1e), `rorelse-uttrycksfull.html` (1d)
- `img/dg-logo-black.png`, `img/dg-logo-white.png` – loggorna (PNG, genomskinlig bakgrund)
- `.htaccess` – noindex-header, ingen mapplistning och (avkommenterbart) lösenordsskydd

## Saknas: de tre fotona (läggs i `img/`)
- `img/gard.jpg` – gården / husen (omslag, 1a, 1b)
- `img/balkonger.jpg` – balkonger i hösten (1a, 1b, 1c)
- `img/fasad.jpg` – fasad med balkonger (index, 1c)
Originalen är ~4 MB per bild: ändra storlek till max ca 1800 px bredd och JPG-kvalitet ~80 innan de läggs in.

## Att göra när sidan läggs på hemsidan
1. Endast nåbar med länk: lägg mappen under en svårgissad sökväg, länka inte till den från menyer eller sitemap och behåll `<meta name="robots" content="noindex, nofollow, noarchive">` i varje sida samt `.htaccess` i mappen. Lägg INTE den hemliga sökvägen i sajtens `robots.txt`: den filen är offentlig och skulle avslöja adressen. Det är inte åtkomstskydd: den som har länken kan öppna sidan. Behövs riktigt skydd, lägg lösenord på mappen.
2. Typsnitt: sidorna hämtar Google Fonts (Familjen Grotesk, Hanken Grotesk, Caveat, Instrument Serif) från Google. Ladda hellre ned och servera dem själva (GDPR).
3. Alla sidor är anpassade för mobil (brytpunkt 820 px) och testade i 390 px och 1280 px bredd: en kolumn, dold meny utom "Mina sidor" och orange ruta under hero-fotot. Testa gärna på riktig telefon.
4. Alla texter, nyheter och tider är exempeltext.
