# Busso! 🃏

Un roguelike di carte basato sul **Tressette** a due, in pixel art.

Affronta cinque avversari in fila — dal Pivellino al Diavolo — accumulando fiche e moltiplicatori, comprando trucchi, poteri magici e amuleti al negozio e arricchendo il mazzo con semi stranieri, Jolly e carte troll.

## Gioca

Il gioco è un'unica pagina HTML, senza installazioni né build:

- **Online:** attiva GitHub Pages (Settings → Pages → Deploy from a branch → `main` / root) e apri `https://<utente>.github.io/<repo>/`.
- **In locale:** scarica il repository e apri `index.html` nel browser.

Aggiungi `#debug` all'indirizzo per aprire la Galleria debug (tutte le carte, oggetti e avversari, negozio con 999 fiche).

## Come si gioca, in breve

- Tressette con tallone: chi prende pesca per primo. Pareggio = sconfitta.
- Punteggio = **Fiche × Molt**. Assi 30, Tre/Due/figure 10, ultima presa 30.
- Le prese di fila caricano i **trucchi** e fanno scattare le **Strisce** (+1 Molt ogni 3).
- Dopo ogni vittoria: pacchetto da 10 carte → negozio → avversario successivo.

Le regole complete sono in [`docs/design.md`](docs/design.md).

## Struttura

```
index.html      il gioco completo (HTML + CSS + JS)
docs/design.md  documento di design
.nojekyll       serve la pagina su GitHub Pages così com'è
```
