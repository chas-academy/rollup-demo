# Bundling av moduler

I detta repo hittar ni exempel på hur vi kan nyttja exempel verktyg för att slå ihop eller "bundla" moduler i JavaScript.

## För att komma igång
1. Det första du behöver göra är att `git clone` detta repo.
2. Om du inte redan har gjort det måste du nu installera båda verktygen `node` och `npm`. Detta gör man genom att ladda ned rätt installationsfil för respektive operativsystem från följande länk:
  https://nodejs.org/en/download/
3. Efter gjord installation testa att du har fått tillgång till både `node` och `npm` genom att skriva följande två kommandon i ett shell:
    ```bash
    $ node -v
    // din version node visas här
    $ npm -v
    // din version av npm visas här
    ```
4. Gå nu till det klonade repot i ditt shell:
    ```bash
    $ cd /path/to/cloned/rollup-demo
    ```
5. Installera alla _beroenden_ genom att skriva kommandot:
    ```bash
    $ npm install
    ```
6. När det är gjort prova att skapa en bundle genom att skriva kommandot:
    ```bash
    $ npm run bundle
    ```
7. Om det lyckades borde du hitta en fil som heter `public/bundle.js`
8. För att säkerställa att det fungerade kan du öppna `public/index.html` i en webbläsare och konstatera att koden inuti `main.js` faktiskt har ändrat i DOM:en.

### Okej, vad gör jag nu?
Nu kan du prova dig fram och skapa egna moduler, importera och exportera för att lära dig mer.


## Vad gör de olika sakerna?
- **node & npm**:
  - Vi använder npm (som använder sig av node) för att installera och använda oss av av moduler som är skrivna av andra utvecklare. Dessa kallas fint för  _beroenden_.
- **rollup**:
  - Vi använder rollup för att slå samman våra