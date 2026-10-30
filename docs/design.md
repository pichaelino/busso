# Busso! — Tressette roguelike (v3)

## Stile
- Carte in pixel art più dettagliate. Denari oro con rosone verde, Coppe rosse con bordo d'oro: i due semi non si confondono più.
- Niente effetto televisore: sfondo fisso a piastrelle di maiolica, colore diverso per ogni avversario.
- Testo in Rubik (leggibile, minuscolo); titoli e numeri in Pixelify Sans. Niente tutto-maiuscolo.

## Struttura della run
- Tressette a due con tallone. Chi prende pesca per primo; le pescate restano coperte. La mano avversaria è in ordine casuale.
- 5 avversari in fila: Pivellino (×1), Zia Assunta (×1.5), Il Baro (×2), Il Vecchietto del Bar (×2.25), Il Diavolo (×2.75). Pareggio = sconfitta.
- Dal 2° avversario in poi c'è una **mossa** che scatta ogni 3 sue prese di fila (Zia +0.25 Molt, Baro ruba la tua carta migliore, Vecchietto ti rimischia la mano nel tallone, Diavolo brucia la tua presa più preziosa).
- Dopo ogni vittoria: riepilogo → pacchetto da 10 carte → negozio → prossimo avversario.

## Punteggio
- Fiche: Asso 30, Tre/Due/figure 10, scartine 0, ultima presa 30. Totale = Fiche × Molt.
- Accusi iniziali; giocate: Strozzo +0.5, Striscia (ogni 3 prese di fila) +1, Piombo +0.5.

## Economia
- Guadagno per vittoria = 120 + distacco (fino a +110, in base al rapporto tra il tuo totale e il suo) + 10 per obiettivo (max +30). Tetto 260 (290 con Salvadanaio).
- Prezzi: poteri 95–110, trucchi 110–135, amuleti 120–160 (+0/5/10 a caso).
- Risultato: una vittoria normale paga un oggetto, una vittoria larga ne paga al massimo due. Le fiche non spese restano.
- Rimescola vetrina 25 (+10 ogni volta). Togli una carta dal mazzo 45, una volta per negozio, mazzo minimo 30.

## Trucchi (si caricano con le prese di fila, max 4)
Soglia S: a S prese di fila liv 1, a 2S liv 2, a 3S liv 3. Usarlo consuma la carica.
Occhio Lungo (2), Sbirciata (2), Tintura (3), Mano Lesta (3), Pesca Truccata (3), Raddoppio (4).

## Poteri magici (monouso, max 3)
Mano del Ladro, Pioggia d'Assi, Ribaltone, Terremoto, Malocchio, Fiammifero.

## Amuleti (passivi, max 5)
Corno Rosso, Ferro di Cavallo, Gatto Nero, L'Oste, Ruota della Fortuna, Scartine d'Oro, Lente, Sigaro del Nonno, Calamita, Salvadanaio (+30 fiche a vittoria).

## Negozio
Sempre almeno 1 trucco, 1 amuleto, 1 potere + 1 casuale.

## Pacchetti (10 carte)
3 semi stranieri (Cuori, Quadri, Fiori, Picche), 3 doppioni toscani, 2 Jolly, 1 troll, 1 a caso. Ne scegli fino a 3; la prima troll del pacchetto entra comunque.
- Jolly: si gioca sempre, scegli il seme quando la cali.
- Tre Marcio: vale come un Tre, chi lo prende perde 40.
- Bomba: si gioca sempre, fa saltare la presa.
- Spettro: si gioca sempre, non prende mai, chi lo raccoglie perde 20.
- Tallone dispari: l'ultima carta rimasta va bruciata.

## Debug
Pagina "Galleria debug" (titolo o link con #debug): tutte le carte, oggetti, avversari, obiettivi; prova un oggetto contro un avversario scelto, partita con tutto, apri pacchetto, negozio con 999 fiche.

## Idee per i prossimi passi
- Personaggi giocabili con abilità di partenza diverse.
- Altri troll e pacchetti a tema.
- Salvataggio della run, statistiche, difficoltà crescente nei giri successivi.
