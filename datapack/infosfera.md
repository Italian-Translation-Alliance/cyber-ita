---
layout: default
title: Infosfera
parent: Datapack
nav_order: 2
---

# Infosfera

## Generatore di nodi dell'infosfera

1. Identificare o tirare la classe di sicurezza
2. Specificare le abilità e le caratteristiche di sicurezza
3. Selezionare o tirare per l'aspetto che si desidera
4. Selezionare o tirare  i dati conservati sul nodo

[Generatore online](https://oswida.github.io/cyber/app/dist/#/gen?lang=en&mode=Infosphere)

## Classe di sicurezza

1. Pubblico
2. Privato
3. Privato protetto
4. Governo
5. Corporazione
6. Militare
7. IA

## Abilità e caratteristiche di sicurezza

Ogni nodo dell'Infosfera ha le abilità PF, INF e parametri aggiuntivi relativi alle sue procedure di sicurezza.
Riducendo a zero i PF di un nodo se ne prende il controllo, riducendo a zero la INF si distruggono i dati.
La seguente tabella indica le capacità e i meccanismi di protezione per ogni classe di sicurezza.

- I `PF` e la `INF` specificano il dado da utilizzare per tirare il valore dell'abilità (insieme al modificatore)
- L'`ICE` determina il dado di attacco per l'Intrusion Countermeasure Electronics e determina la possibilità che un dato ICE sia "black" (tirando il Dado del Fato, x/6 significa che i risultati da 1 a x danno una risposta positiva).
- La `Soglia di attivazione` definisce il valore massimo che attiva il programma di protezione aggiuntivo in un dato round.

| Classe di sicurezza |   PF  | INF | Soglia di attivazione | Dado attacco ICE |
| ------------------- |:-----:|:---:|:---------------------:|:----------------:|
| Pubblico            |  d4+1 |  d4 |           1           |        d4        |
| Privato             |  d4+1 |  d4 |           2           |        d4        |
| Privato protetto    |  d6+2 |  d6 |           3           |        d6        |
| Governo             |  d8+3 |  d8 |           5           |  d8, 1/6: Black  |
| Corporazione        | d10+4 | d10 |           7           |  d10, 2/6: Black |
| Militare            | d12+5 | d12 |           9           |  d12, 3/6: Black |
| IA                  | d20+6 | d20 |           12          |  d20, 4/6: Black |

### Software di protezione aggiuntivo

Ogni nodo può disporre di un software di protezione aggiuntivo. La sua attivazione non è necessariamente inevitabile e dipende dal risultato del tiro durante l'attacco dell'ICE.
La procedura non richiede alcun tiro di dadi aggiuntivo: il valore viene indicato dall'attacco dell'ICE. Se il risultato del tiro è minore o uguale alla soglia di attivazione, nello stesso round viene lanciato il programma e il suo tipo viene indicato dal software di protezione tabella, anche in base al valore di attacco.

| d4 - d20 | Software di protezione                                          |
|:--------:| --------------------------------------------------------------- |
|     1    | PF +1 (*)                                                       |
|     2    | PF +2 (*)                                                       |
|     3    | PF +3 (*)                                                       |
|     4    | Armatura +1                                                     |
|     5    | Armatura +2                                                     |
|     6    | Armatura +3                                                     |
|     7    | Dispersione: il prossimo attacco dell'hacker è compromesso      |
|     8    | Danno critico: d4 danni aggiuntivi                              |
|     9    | Danno critico: l'attacco dell'hacker è compromesso per d4 round |
|    10    | Danno critico: l'hacker è disconnesso per d4 round              |
|    11    | Firewall: incapacità di hackerare nel round successivo          |
|    12    | Doppio attacco (tira due dadi, scegli il risultato più alto)    |

(*) Se al momento dell'aumento dei PF l'hacker controllava il nodo, ne perde il controllo fino a quando non riduce nuovamente a zero i PF del nodo.

> Esempio di attivazione del software di protezione
>
> Ian attacca il nodo corporativo, il che significa che l'ICE ha d10 dadi di attacco.
> Inoltre, il tiro del d6 dà un risultato di 2: significa che l'ICE attaccato è "black" (in caso di fallimento della prova di danno critico, Ian riceverà danni PSI aggiuntivi)
> Al momento dell'attacco, l'ICE tira un 5. Significa che:
>
> - Ian riceverà **5 punti danno** (prima li sottrae dai suoi PF e poi dalla sua INF).
> - È stato **attivato** un ulteriore programma di protezione (soglia di attivazione 7)
> - L'effetto del programma di protezione è **+2 armatura** in questo round (**riga 5** nella tabella), il danno inflitto al nodo da Ian sarà ridotto di 2 (l'attacco dell'hacker e del nodo vengono risolti simultaneamente)

## Aspetto (3d20)

| d20 | Forma                  | Colore e/o materiale            | Dettagli                                                |
| --- | ---------------------- | ------------------------------- | ------------------------------------------------------- |
| 1   | Sfera                  | Rubino, trasparente             | Raggi laser che riempiono la forma                      |
| 2   | Piramide/ziggurat      | Trasparente                     | Simboli matematici visualizzati sulla superficie        |
| 3   | Simbolo di infinito    | Nero, opaco                     | Brucia con luce intensa                                 |
| 4   | Cubo                   | Argento                         | Anelli luminosi che turbinano                           |
| 5   | Mock-up di un edificio | Verde, neon                     | Slogan pubblicitari affissi in facciata                 |
| 6   | Maschera               | Bianco, lucido                  | Ricorda gli origami                                     |
| 7   | Menhir                 | Nero, lucido                    | Pieno di fulmini                                        |
| 8   | Cerchio                | Blu, incandescente              | Pieno di cristalli di ghiaccio                          |
| 9   | Modello di un atomo    | Grigio, pietroso                | Senza contrassegni aggiuntivi                           |
| 10  | Marchio                | Blu, nebbioso                   | Logo grande azienda/proprietario                        |
| 11  | Nastro di Moebius      | Verde, luminoso                 | Cubi luminosi all'interno                               |
| 12  | Cubo di Rubik          | Rosso, fiammeggiante            | Simboli mistici che turbinano                           |
| 13  | Schermo                | Multicolore                     | Puntini di luce che appaiono casualmente                |
| 14  | Vortice                | Oro                             | Immagini della griglia casuali visualizzate all'interno |
| 15  | Colonna                | Metallico, lucido               | Avvolto in una griglia metallica                        |
| 16  | Triangolo              | Blu scuro, coperto di striature | Lampeggiante regolarmente con luce fioca                |
| 17  | Occhio                 | Vetro, trasparente              | Gira intorno al proprio asse                            |
| 18  | Cancello               | pezzato, marrone                | Segmenti rotanti continuamente                          |
| 19  | Trapezio               | Arancione, luminoso             | Frattali dinamici disegnati sulla superficie            |
| 20  | Perpendicolare         | Acciaio, ricoperto di simboli   | Ogni tanto scompare e riappare                          |

## Dati da acquisire (d20)

Se i tuoi hacker stanno irrompendo nei nodi dell'Infosfera per mettere le mani su dati preziosi, le seguenti tabelle potrebbero fornire ispirazione.

### Pubblico

1. Una serie di vecchi giochi per computer
2. Grande libro di ricette
3. Piante di un edificio pubblico
4. Risposte alle domande del prossimo quiz multimediale
5. Trucchi per un popolare gioco online
6. Ricetta per stimolanti fatti in casa
7. Un volume di poesie di discutibile qualità
8. Disegni molto interessanti di vestiti alla moda
9. Elenco dei vincitori di un concorso di bellezza che non ha ancora avuto luogo
10. La più grande collezione di musica al mondo
11. Dati crittografati sconosciuti
12. Registrazione della telecamera di sicurezza dell'edificio pubblico
13. Orario di una nota star dei media
14. Filmato di un violento intervento della polizia
15. Filmati di proteste di attivisti al cancello della fabbrica
16. Filmato del manifesto di un gruppo terroristico
17. Dichiarazione ufficiale del gruppo hacker
18. Dati medici completi su un farmaco per una malattia nota
19. Progetti tecnici per un drone della polizia
20. Elenco degli agenti di polizia corrotti

### Privato

1. Dati medici rubati dall'ospedale amministrativo
2. Piani tecnici di una cybermodifica sconosciuta
3. Raccolta di video... di vario genere
4. Una raccolta di articoli su misteriosi esperimenti genetici
5. 1d4 biglietti per un famoso evento sportivo
6. Una serie di 1d4 virus informatici
7. Manoscritto di un romanzo inedito (potrebbe andar bene)
8. Codici di accesso ad un appartamento privato
9. Corrispondenza con una società in materia di risarcimento
10. Archivio dati su una nota celebrità
11. Cartelle cliniche indicanti una malattia incurabile
12. Codici di lancio per un veicolo privato
13. Manifesto redatto di un gruppo terroristico
14. Guida su come realizzare una bomba
15. Una raccolta di email d'amore
16. Ultimo testamento autorizzato
17. Inviti di nozze e lista degli invitati
18. Foto di una clinica informatica illegale
19. Riprese amatoriali di un hack
20. Canzone sconosciuta di un famoso gruppo musicale

### Privato protetto

1. Una serie di documenti falsi
2. 1d4 firme false per veicoli di qualsiasi tipo
3. Coordinate bancarie con 1k4 mila crediti
4. 1d4 biglietti per un prossimo concerto al teatro dell'opera
5. 1d6 programmi di hacking di vario tipo
6. Codici per l'hacking delle linee elettriche nel distretto selezionato
7. Immettere i codici per diversi appartamenti in un normale grattacielo
8. Indirizzi di famiglie di noti capibanda
9. Due pass per un ristorante esclusivo
10. Codici di accesso ad un garage privato
11. Password per l'account di posta elettronica aziendale
12. Chiave elettronica per d6 armadietti delle armi
13. Diario di un importante politico
14. Elenco dei contatti della star dei media
15. Indirizzo di rete di un dirigente aziendale
16. Immettere il codice in una delle arcologie aziendali
17. Password per un account con un abbonamento Platinum Basic
18. Codici di accesso per un deposito di stimolanti illegali
19. Indirizzo di contatto di un fixer noto
20. Documento di ricevuta per cybermodifica/drone da combattimento

### Governo

1. Codici per aprire tutte le porte dell'Amministrazione selezionata
2. Registrazione della telecamera di sicurezza con crimine registrato
3. Piani di evacuazione in caso di epidemia di una malattia infettiva pubblicamente sconosciuta
4. Relazione sugli animali mutanti incontrati dai lavoratori comunali
5. Testimonianze finanziarie di noti politici
6. Ultimatum del gruppo terroristico che minaccia la contaminazione chimica
7. Dati finanziari che indicano una crisi economica imminente
8. Rapporto sulla contaminazione radioattiva in un quartiere della città
9. Informazioni sulla cessazione dei diritti della società sul terreno occupato dalla fabbrica
10. Planimetrie dettagliate del quartiere cittadino selezionato
11. Atto di proprietà di una piccola proprietà comunale
12. Immissione di codici per il sistema ospedaliero amministrativo
13. Rapporto sul bizzarro comportamento dell'IA che gestisce il trasporto urbano
14. 1k6 permessi per l'esercizio del trasporto pubblico (vuoto)
15. Calendario delle interruzioni delle linee elettriche in diverse parti della città
16. Bozza della nuova legge tributaria per i cittadini
17. Immissione di codici per il magazzino dell'ospedale cittadino
18. Password e codici che entrano in emergenza epidemiologica
19. 1d4 moduli in bianco che consentono la registrazione dell'identità
20. Codici di accesso per il sistema di controllo dei servizi comunali selezionati

### Corporazione

1. Gli ultimi episodi ancora da trasmettere di una serie popolare
2. Registrazioni compromettenti di un importante dipendente aziendale
3. Pianta dettagliata di una delle arcologie della corporazione
4. Informazioni personali di un intero dipartimento aziendale
5. Elenco dei conti bancari di un noto dipendente aziendale
6. Documentazione di produzione di un vaccino raro
7. Dati dei dipendenti sospettati di spionaggio
8. Fascicoli personali dei dipendenti di una società rivale
9. Set di tessere d'ingresso per arcologia
10. Dati compromettenti dei politici
11. Dati tecnici dell'ultimo prodotto dell'azienda
12. Informazioni sul finanziamento di gruppi terroristici
13. Elenco degli agenti di polizia al servizio dell'ente
14. Elenco dei funzionari dell'Amministrazione al servizio dell'ente
15. Piani per prendere il controllo delle bande nel distretto
16. Contatti con persone/aziende assunte per 'lavoro bagnato'
17. Documentazione di esperimenti genetici illegali
18. Password per un magazzino pieno di prodotti della società
19. Ordini di trasporto di materiali sconosciuti a una struttura di ricerca
20. Progetti per una struttura di ricerca aziendale

### Militare

1. Technical plans of the combat drone
2. Input codes for military base
3. Remote control codes for a military fighter jet
4. Program decrypting transmissions on tactical network
5. Technical plans for a military robot
6. Weapons storage input codes
7. Pass codes to the military cybermod warehouse
8. Address data of important military commanders
9. Production documentation of military stimulants
10. Military satellite control codes
11. Satellite images showing illegal research facilities
12. List of competitor spies in a selected corporation
13. Orders to exterminate the population in case of an unknown disease threat
14. Documentation of a deadly virus grown in a laboratory
15. Nuclear warhead deployment plans
16. Transcripts of discussions of meetings of the board of directors of a selected corporation
17. List of corporate AIs perceived as a threat
18. Technical plans for a super-light EMP weapon
19. Technical plans for the EMP-emitting cyber-arm
20. List of military spies in corporations

1. Schemi tecnici del drone da combattimento
2. Immissione di codici per una base militare
3. Codici di telecomando per un caccia militare
4. Programmare la decrittografia delle trasmissioni sulla rete tattica
5. Progetti tecnici per un robot militare
6. Codici di input del deposito di armi
7. Passa i codici al magazzino cybermodifiche militare
8. Indirizzo dati di importanti comandanti militari
9. Documentazione di produzione di stimolanti militari
10. Codici di controllo dei satelliti militari
11. Immagini satellitari che mostrano strutture di ricerca illegali
12. Elenco delle spie concorrenti in una società selezionata
13. Ordini di sterminio della popolazione in caso di minaccia di malattia sconosciuta
14. Documentazione di un virus mortale coltivato in laboratorio
15. Piani di spiegamento di testate nucleari
16. Trascrizioni delle discussioni delle riunioni del consiglio di amministrazione di una società selezionata
17. Elenco delle IA aziendali percepite come una minaccia
18. Piani tecnici per un'arma EMP superleggera
19. Piani tecnici per il cyber-braccio che emette EMP
20. Elenco delle spie militari nelle corporazioni

### IA

1. Costrutto (personalità registrata) di una celebrità deceduta
2. Dati tecnici del nodo dell'Agenzia per l'energia atomica
3. Codici sorgente di un'altra IA
4. Immettere i codici in tutti i sistemi di polizia
5. Set di 1d6 potenti virus informatici
6. Password per un nodo completamente resistente all'hacking
7. Password per un account anonimo con 1d20k crediti 
8. Procedura per l'accesso una tantum a qualsiasi nodo dell'Infosfera
9. Un virus che spegne i sistemi di sicurezza nell'edificio indicato per 1d20 minuti
10. Codici di controllo automatico dei veicoli militari
11. Codici di controllo del sistema di trasporto pubblico
12. Ricetta per stimolante che crea dipendenza k10
13. Codici per un missile intercontinentale con testate nucleari
14. Dati medici di un esperimento relativo all'immortalità umana
15. Dati di una struttura di ricerca segreta che alleva mutanti umani
16. Virus che blocca completamente le trasmissioni della rete multimediale selezionata
17. Piani militari segreti per attaccare una delle corporazioni
18. Prova che una società è completamente gestita dall'intelligenza artificiale
19. Piano di attacco all'Infosfera da eseguire da IA ​​canaglia
20. Un virus distruttivo, che cancella istantaneamente tutti i dati sul nodo su cui è stato lanciato

# Algoritmi di base

## Azioni dei PG

![Azioni dei PG](img/Azioni%20dei%20PG.svg)

## Combattimento fisico

![Combattimento fisico](img/Combattimento%20fisico.svg)

## Attacco al nodo dell'infosfera

![Attacco nell'Infosfera](img/Attacco%20nell'Infosfera.svg)

## Attacco ICE

![Attacco ICE](img/Attacco%20ICE.svg)

# Algoritmi aggiuntivi

Diversi meccanismi aggiuntivi per espandere le giocate nell'Infosfera.

## Scontri tra hacker

La versione base del gioco presuppone che gli hacker possano attaccare i nodi nell'Infosfera ed essere attaccati dagli Intrusion Countermeasure Electronics.
Ma cosa succede se si incontrano diversi hacker di fazioni opposte?
Il neuroprocessore conferisce all'hacker una capacità molto maggiore di gestire l'Infosfera ma allo stesso tempo lo espone ad attacchi diretti dalla rete.

It is possible to attack the hacker's mind in a similar way to the Infosphere node.
Such an action has to be performed by another hacker; no software can do it. There are rumors that some AI also happened to attack the human mind.

È possibile attaccare la mente dell'hacker in modo simile al nodo di Infosfera.
Tale azione deve essere eseguita da un altro hacker; nessun software può farlo. Si dice che anche alcune IA abbiano attaccato la mente umana.

Lo scontro segue le stesse regole dei nodi. Gli avversari **attaccano con i neuroprocessori** e il danno viene inflitto prima ai PF dell'avversario e poi all'INF. Gli attacchi avvengono simultaneamente.
Ridurre l'OCHR dell'hacker a zero o meno significa che l'altra parte può **assumere il controllo degli stimoli** ricevuti dalla parte sconfitta per **tanti round quanti sono i punti di INF**.

Prendere il controllo si applica solo al sensorio dell'hacker (vista, udito, olfatto), non include i motori, ad es. non puoi controllare il corpo dell'avversario. Ma puoi invece controllare completamente la sua percezione.

## Supporto

Se due o più hacker desiderano coordinare le loro azioni quando attaccano un nodo, le loro azioni sono considerate allo stesso modo dell'attacco multiplo nelle regole di combattimento.
Tira **tutti** i dadi di danno e **scegli** un risultato.
La differenza con il combattimento fisico (dove viene considerato il punteggio più alto) è che gli hacker possono modificare l'effetto di un attacco con i programmi. Quando si risolve l'attacco, **solo quei programmi** che appartengono al **proprietario del tiro selezionato** possono essere attivati.

## Passeggeri

Qualsiasi hacker può connettere qualsiasi numero di dispositivi di accesso ordinari al suo neuroprocessore. In questo modo, gli estranei che non dispongono di un neuroprocessore possono avere un contatto costante con lui e persino osservare le sue attività online. Tuttavia, nessuno dei passeggeri può intraprendere alcuna azione nell'Infosfera; la loro partecipazione è limitata solo all'osservazione passiva o alla comunicazione con l'hacker.