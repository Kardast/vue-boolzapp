# vue-boolzapp
Eccoci,
Esercizio lungo che parte oggi e ci portiamo fino a martedì prossimo,
quindi prima consegna entro martedì verso le 17/17-30 massimo.
(Ricordatevi però di far sempre commit e push frequenti e sensati)
Mercoledì poi potrete andarci comunque avanti.
nome repo: vue-boolzapp
Doc di specifiche:
https://docs.google.com/document/d/1n7zAM-rjfdqDIzszFA1F6pSZDL4LADU4w8k1RAl8kzM/edit?usp=sharing
Per il resto come sempre:
sia mattina che pome ticket,
ma comunque sia mattina di lunedì che di martedì, ci vediamo in aula alla solita ora per vedere se ci sono grossi dubbi.
Buon lavoro e we.


Possibili bonus (oltre il principale segnato sul doc di specifiche):
Come sempre se equando avrete finito tutto il resto,
ma ve le giro così potete metterle li da parte.
Come detto fate prima un bel refactoring in caso generale, sperando l’abbiate fatto anche man mano che sviluppavate i milestones principali.
Codice:
se ho messo qualche v-if in qualche v-for, cercare una alaternativa (in questo caso datevi un’occhiata alle “computer properties”, è una delle possibili utilità);
Funzionalità
evitare che l’utente possa inviare un messaggio vuoto o composto solamente da spazi
A) cambiare icona in basso a destra (a fianco all’input per scrivere un nuovo messaggio) finché l’utente sta scrivendo: di default si visualizza l’icona del microfono, quando l’input non è vuoto si visualizza l’icona dell’aeroplano. Quando il messaggio è stato inviato e l’input si svuota, si torna a visualizzare il microfono. B) inviare quindi il messaggio anche cliccando sull’icona dell’aeroplano
predisporre una lista di frasi e/o citazioni da utilizzare al posto della risposta “ok:” quando il pc risponde, anziché scrivere “ok”, scegliere una frase random dalla lista e utilizzarla come testo del messaggio di risposta del pc
visualizzare nella lista dei contatti l’ultimo messaggio inviato/ricevuto da ciascun contatto
inserire l’orario corretto nei messaggi (v. note day.js)
sotto al nome del contatto nella parte in alto a destra, cambiare l’indicazione dello stato: visualizzare il testo “sta scrivendo...” nel timeout in cui il pc risponde, poi mantenere la scritta “online” per un paio di secondi e infine visualizzare “ultimo accesso alle xx:yy” con l’orario corretto
dare la possibilità all’utente di cancellare tutti i messaggi di un contatto o di cancellare l’intera chat con tutti i suoi dati: cliccando sull’icona con i tre pallini in alto a destra, si apre un dropdown menu in cui sono presenti le voci “Elimina messaggi” ed “Elimina chat”; cliccando su di essi si cancellano rispettivamente tutti i messaggi di quel contatto (quindi rimane la conversazione vuota) oppure l’intera chat comprensiva di tutti i dati del contatto oltre che tutti i suoi messaggi (quindi sparisce il contatto anche dalla lista di sinistra)
dare la possibilità all’utente di aggiungere una nuova conversazione, inserendo in un popup il nome e il link all’icona del nuovo contatto
fare scroll in giù in automatico fino al messaggio più recente, quando viene aggiunto un nuovo messaggio alla conversazione (NB: potrebbe esserci bisogno di utilizzare nextTick: https://vuejs.org/v2/api/#Vue-nextTick)
aggiungere le emoticons, tramite l’utilizzo di una libreria, ad esempio: https://www.npmjs.com/package/vue-emoji-picker
Grafica
visualizzare un messaggio di benvenuto che invita l’utente a selezionare un contatto dalla lista per visualizzare i suoi messaggi, anziché attivare di default la prima conversazione
aggiungere una splash page visibile per 1s all’apertura dell’app
A) rendere l’app responsive e fruibile anche su mobile: di default si visualizza solo la lista dei contatti e cliccando su un contatto si vedono i messaggi di quel contatto. B) aggiungere quindi un’icona con una freccia verso sinistra per tornare indietro, dalla visualizzazione della chat alla visualizzazione di tutti i contatti
aggiungere un’icona per ingrandire o rimpicciolire il font: dovrebbe essere sufficiente aggiungere una classe al wrapper principale
aggiungere un’icona per cambiare la modalità light/dark: dovrebbe essere sufficiente aggiungere una classe al wrapper principale
Per la gestione delle date,
potrebbe servirvi la libreria che avevam visto già venerdi al volo, con le seguenti considerazioni:
https://day.js.org/
Per poter leggere una data in un formato diverso dal formato standard ISO 8601, è necessario aggiungere a day.js il plugin CustomParseFormat: https://day.js.org/docs/en/parse/string-format
Per installarlo, recuperare il link alla cdn e usaro come in questo esempio: https://day.js.org/docs/en/plugin/loading-into-browser
Il supporto dei ticket chiaramente avrà priorità sui milestones base. :pulcino_appena_nato: