# Table Dipartimenti
- Id
- Nome
- Indirizzo
- Email
- Telefono
- Numero corsi di laurea

# Table Corsi di Laurea
- Id
- Nome
- Numero corsi
- Codice corso di laurea
- Tipo
- Requisiti
- Note
- Durata
- Lingua

# Table Corsi
- Id
- Nome
- Durata
- Esami
- Insegnanti
- Studenti
- Note



# Table Insegnanti
- Id
- Nome
- Cognome
- Anno di nascita
- Email
- Note
- Lingua


# Table Esami
- Id
- Nome
- Tipo
- Codice
- Durata
- obbligatorio
- CFU
- Data


# Table Studenti
- Id
- Nome
- Cognome
- Matricola
- Email
- Anno di nascita
- Media voti
- Fascia reddituale
- Occupazione
- Voto diploma
- Note


# Relationships 

Dipartimento <oneToMany> Corsi di laurea 
Corso di Laurea <manyToMany> Corsi 
Corso <manyToMany> Insegnanti 
Corso <oneToMany> Esami
Corso <manyToMany> Studenti
Studente <manyToMany> Esami