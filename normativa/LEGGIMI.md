# Tabelle normative di Quadra

Quadra controlla `https://slaplacah501service-hub.github.io/quadra/normativa/manifest.json`. Se trova una versione più nuova della sua, scarica il pacchetto, ne verifica l'impronta SHA-256 e lo usa al posto di quello incluso nel setup.

## Per pubblicare un aggiornamento
1. Copia l'ultimo `pacchetto-<versione>.json`, cambiane il nome con una versione nuova (per esempio `pacchetto-2027.1.1.json`) e modificalo: aliquote, nature, esenzioni, tipi documento, regimi, modalità di pagamento, bollo, tracciato.
2. Nel file nuovo aggiorna `versione` e `data`.
3. In `manifest.json` metti la nuova `versione`, il nuovo `url` e lo `sha256` del file. Su Windows lo ottieni con `certutil -hashfile pacchetto-2027.1.1.json SHA256`.
4. Carica i due file sulle Pages, nella cartella `normativa/`.

## Fonte ufficiale dei dati
Le specifiche tecniche della fattura elettronica (FatturaPA) dell'Agenzia delle Entrate, su fatturapa.gov.it e agenziaentrate.gov.it.
