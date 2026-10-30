# Busso! — Tressette roguelike (v9)

Un gioco di 10INCH FEET GAMES. All'avvio c'è lo splash dello studio (clic o un tasto per saltarlo).

## Stile
- Carte in pixel art più dettagliate. Denari oro con rosone verde, Coppe rosse con bordo d'oro.
- Il bordo di ogni carta ha il colore del seme: Coppe rosso, Denari oro, Spade blu, Bastoni verde, Cuori rosso, Quadri arancio, Fiori nero, Picche blu notte. Numeri negli angoli più grandi.
- Niente effetto televisore: sfondo fisso a piastrelle di maiolica, colore diverso per ogni avversario.
- Testo e numeri in Rubik (leggibili); titoli in Pixelify Sans. La parola FICHE è sempre in maiuscolo.
- Il pacchetto è un oggetto vero: trema, si strappa in alto, le 10 carte volano fuori e si girano una a una.

## Giocatori (scelti a inizio run, una sola abilità)
- **Il Toscano** — mazzo toscano (Coppe, Denari, Spade, Bastoni). Abilità *Busso!*: se esci con un Tre e vinci la presa, +0.5 Molt.
- **Lo Straniero** — mazzo francese (Cuori, Quadri, Fiori, Picche). Abilità *Doppia valuta*: le figure prese (Fante, Donna, Re) valgono 15 FICHE invece di 10.
- Tecnicamente è una "pelle": i semi di casa restano C/D/B/S nel codice e vengono mostrati come francesi per lo Straniero (Cavallo → Donna). I semi stranieri dei pacchetti diventano quelli toscani. Obiettivi, avversari e amuleti funzionano uguali, con i nomi tradotti.
- Mazzo francese a quattro colori per distinguerli: Cuori rosso, Quadri blu, Fiori verde, Picche nero.

## Partita
- Molt degli avversari (v9): Pivellino ×1.1, Zia ×1.6, Nonna e Don Ottavio ×1.85, Capitano e Baro ×2.1, Prestigiatore e Vecchietto ×2.35, Diavolo ×2.85.
- **Accusi a tasto**: quando hai un accuso in mano compare il tasto *Accusa* (Napoletana 90, tre Tre/Due/Assi 90, passare a quattro aggiunge 30). Lo premi quando vuoi nel tuo turno. L'avversario accusa da solo appena può, e le carte dell'accuso restano scoperte nella sua mano finché non le gioca. Don Ottavio azzera i tuoi accusi.
- *Carte del mazzo* si apre anche in partita, ma mostra solo la composizione: non dice quali carte sono in mano, nel mazzo o già uscite.
- Ritratti senza lacrime. Carte ancora più grandi.
- Il tallone si chiama **Mazzo**.
- Quando una presa finisce compare un'etichetta dal lato di chi la vince ("Presa tua · +40 FICHE" in blu sopra la tua mano, "Presa di … " in oro sotto la sua) e le carte volano verso di lui.
- Carte più grandi. Assi ridisegnati con raggi, corona, alloro e nastro.
- Ritratti rifatti: testoni pallidi, occhi neri lucidi, lacrime e roba che pende.
- Titolo: "Premi F11 per andare a schermo intero".

## Trucchi rivisti
- Occhio Lungo: scopre 1/2/3 sue carte, che restano scoperte finché non le gioca.
- Sbirciata: liv 1 vedi la prima del mazzo, liv 2 prime 2 e puoi invertirle, liv 3 prime 3 e scegli la prima.
- Mano Lesta: liv 1 una carta con una sua a caso, liv 2 una carta scegliendo tra le sue scoperte, liv 3 due carte.

## Struttura della run
- Tressette a due con tallone. Chi prende pesca per primo; le pescate restano coperte. La mano avversaria è in ordine casuale.
- Sempre 5 partite: si comincia col Pivellino e si finisce col Diavolo. In mezzo 3 avversari a caso tra Zia Assunta, Nonna Pina, Don Ottavio, Il Capitano, Il Baro, Il Prestigiatore e Il Vecchietto del Bar.
- Ogni avversario dal 2° in poi ha una **mossa** che scatta ogni 3 sue prese di fila.
- Obiettivi: 2 nelle prime due partite (in versione più facile), 3 dalla terza in poi, presi da un elenco di 28.
- Dopo ogni vittoria: riepilogo → pacchetto da 10 carte → negozio → prossimo avversario.
- Esc (o il pulsante Menu) apre la pausa: torna alla partita, musica sì/no, effetti sì/no, ricomincia la run (con conferma). In pausa l'avversario si ferma.
- Musica chiptune generata nel browser, diversa tra titolo, partita, negozio e Diavolo.

## Punteggio
- Fiche: Asso 30, Tre/Due/figure 10, scartine 0, ultima presa 30. Totale = Fiche × Molt.
- Accusi iniziali; giocate: Strozzo +0.5, Striscia (ogni 3 prese di fila) +1, Piombo +0.5.

## Economia
- Guadagno per vittoria = 120 + distacco (fino a +110, in base al rapporto tra il tuo totale e il suo) + 10 per obiettivo (max +30). Tetto 260 (290 con Salvadanaio).
- Prezzi (v7, +15%): poteri ~180–215, trucchi ~205–255, amuleti ~225–305. Carte singole 40–140, pacchetto 175.
- Con questi prezzi una vittoria di misura spesso non basta per un oggetto: conviene risparmiare o vincere largo. Le FICHE non spese restano.
- Rimescola vetrina 25 (+10 ogni volta). Togli una carta dal mazzo 200, una volta per negozio, mazzo minimo 30.

## Identità visiva (v8)
- Colonna sinistra: foto segnaletica dell'avversario (polaroid con nastro), **lavagna da bar** col punteggio scritto a gesso (FICHE × Molt = totale, poi l'avversario, prese), obiettivi, amuleti e cronaca su **scontrini**.
- Ogni avversario ha il suo **tavolo**: tovaglia/panno con motivo e due oggetti negli angoli.
  Pivellino panno verde, lattina e telefono crepato · Zia Assunta tovaglia a fiori, flacone di pillole e moka · Nonna Pina tovaglia a quadri, piatto di pasta e mattarello · Don Ottavio velluto viola con croci, rosario e candela · Il Capitano assi di legno, rum e bussola · Il Baro panno da bisca, dadi e posacenere · Il Prestigiatore velluto nero stellato, cilindro col coniglio e bacchetta · Il Vecchietto formica da bar, bicchiere di rosso e giornale · Il Diavolo pietra con crepe di fuoco, teschio con candela e contratto che brucia.
- La carta appena pescata è evidenziata nella mano (alone dorato, etichetta "Nuova").
- Trucchi e poteri in colonna a sinistra del Mazzo (due colonne quando sono più di 3); l'accuso è un pulsante rosso grande accanto al suggerimento.
- Contatore delle prese di fila: fiamma che si accende, numero grande e tre tacche verso la prossima Striscia.
- La cronaca della partita si apre dal menu di pausa (Esc).
- Lavagna e scontrini su carta più scura, niente bianco acceso. Niente selezione del testo col doppio clic.

## Livelli degli oggetti (0–4)
- Ogni oggetto ha un livello. Il negozio propone livelli diversi a seconda di quanto sei avanti: dopo la 1ª vittoria 0–2, dopo la 2ª 1–3, poi 2–4.
- Prezzi per livello — amuleti 90/150/220/300/400, trucchi 110/170/230/290/360, poteri 80/130/180/230/290.
- **Amuleti a famiglie**: lo stesso amuleto esiste a più livelli e cresce di potenza. Comprarne uno di livello più alto sostituisce quello che hai.
  Corno Rosso (+0.25/+0.5/+1/+1.5/+2.5 Molt) · Ferro di Cavallo (×1.1→×2) · Gatto Nero (+20→+150 sull'ultima presa) · L'Oste (+2→+14 a Coppa) · Ruota della Fortuna (+0.1→+1 per Asso) · Scartine d'Oro (2→14) · Grappa della Casa (+0.1→+1 per Re) · Sigaro del Nonno (+0.25→+2 per obiettivo) · Salvadanaio (+10→+80 a vittoria) · Quadrifoglio (+0.05→+0.6 per carta straniera) · Orologio del Bar (ultime 1→5 prese doppie) · Santino (troll −25%→annullate, al liv 4 danno +10) · Ventaglio (Striscia +0.25→+1.5 Molt) · Pergamena (accusi +10%→+100%) · Lente (prima carta solo dopo una presa vinta → fino a 3 carte) · Calamita (liv 2–4).
  Livelli 0 e 1: 15 amuleti ciascuno; livelli 2–4: 16.
- **A inizio run** scegli un amuleto tra tre di livello 0 o 1.
- Livelli di trucchi e poteri: Fiammifero e Monetina 0 · Occhio Lungo, Sbirciata, Spinta, Pioggia d'Assi, Calice, Grappino 1 · Tintura, Pesca, Raddoppio, Malocchio, Nebbia, Terremoto, Acquasanta 2 · Mano Lesta, Mano del Ladro, Specchio 3 · Bacchetta, Ribaltone 4.
- Nuovi poteri: Monetina (+40 FICHE), Grappino (+0.5 Molt), Acquasanta (annulla la prossima mossa dell'avversario).

## Trucchi (si caricano con le prese di fila, max 4)
Soglia S: a S prese di fila liv 1, a 2S liv 2, a 3S liv 3. Usarlo consuma la carica.
Occhio Lungo (2), Sbirciata (2), Tintura (3), Mano Lesta (3), Pesca Truccata (3), Raddoppio (4).

## Poteri magici (monouso, max 3)
Mano del Ladro, Pioggia d'Assi, Ribaltone, Terremoto, Malocchio, Fiammifero.

## Amuleti (passivi, max 5)
Corno Rosso, Ferro di Cavallo, Gatto Nero, L'Oste, Ruota della Fortuna, Scartine d'Oro, Lente, Sigaro del Nonno, Calamita, Salvadanaio (+30 fiche a vittoria).

## Negozio
Sempre almeno 1 trucco, 1 amuleto, 1 potere + 1 casuale. Un oggetto visto in vetrina non torna più nella stessa run.
Vende anche 2 carte singole (scartine 40, figure 60, Due e Tre 75, Assi 95, semi stranieri +20, Jolly 140) e un pacchetto da 10 carte (175 FICHE). Il negozio sta in una schermata sola, senza scorrere.

## Seme delle Ossa
- Nuovo seme a tema (Ossa, simbolo teschio e ossa incrociate, bordo viola). Ogni carta di Ossa vale 5 FICHE in più a chi la prende; chi non ha Ossa non può rispondere.
- Si trova nella **Cassetta del Becchino** (6 Ossa, 1 Jolly, 1 troll a caso, 1 Spettro, 1 tra Ossa e Jolly) e a volte come carta singola in bottega.
- Il Jolly si può giocare solo come uno dei semi ancora in gioco (mani e Mazzo).

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
