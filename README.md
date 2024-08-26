# Milestone 0
Progettare la struttura del global state sulla linea degli esercizi svolti nei giorni precedenti.
- Inizializzo il progetto con vue + vite
- Creo file store.js
- Importo reactive da vue
- Creo oggetto con vari endpoint che voglio utilizzare

# Milestone 1:
Creare un layout base con una searchbar (una input e un button) in cui possiamo scrivere completamente o parzialmente il nome di un film. Possiamo, cliccando il
bottone, cercare sull’API tutti i film che contengono ciò che ha scritto l’utente. Vogliamo dopo la risposta dell’API visualizzare a schermo i seguenti valori per ogni
film trovato:
1. Titolo
2. Titolo Originale
3. Lingua
4. Voto

- Creo delle componenti Header e Main
- Nell'Header, creo un campo input e un button per la ricerca di un film
- Creo una direttiva v-model alla quale associo una variabile stringa vuota contenuta in store.js
- Invio una richiesta all'App.vue passando come parametro la stringa inserita dall'utente
- In App.vue, eseguo la chiamata axios e popolo l'array vuoto, creato in store, con gli oggetti corrispondenti alla richiesta dell'utente
- Creo la props per passare l'array al Main, dove popolo le ul con i dati richiesti