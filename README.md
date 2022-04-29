# db-sql-1

- studio delle slide
- recupero della registrazione video per assenza

- 1 selezionare tutti gli insegnanti
> SELECT * FROM teachers; //ossia seleziona ogni valore in colonna teachers

- 2 seleziona tutti i capi di ogni dipartimento
> SELECT head_of_department FROM department // same

- 3 selezionare tutti i corsi di laurea magistrae
> SELECT * FROM degrees WHERE level = 'magistrale'  // prende solo ('), non (")

- 4 slezionare tutti gli studenti che hanno come nome Marco
> SELECT * FROM students WHERE name ='Marco' //stesso principio

- 5 selezionare tutti i corsi che valgono uguale o maggiore a 12 crediti
> SELECT * FROM courses WHERE cfu >= 12 // uguale, con il principio di > e =

- 6 selezionare tutti i corsi che valgono più di 10 cfu o meno di 5 cfu
> SELECT * FROM courses WHERE cfu > 10 OR cfu < 5 // condizione a OR b

- 7 Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso
> SELECT * FROM courses WHERE year = 1 AND period = 'I semestre'  //operatore AND

-8 Selezionare tutti i corsi(insegnamenti)  che non hanno un sito web 
> SELECT * FROM courses WHERE website IS NULL // non (= NULL) ma IS NULL

-9 Selezionare tutti gli insegnanti che hanno un numero di telefono
> SELECT * FROM teachers WHERE phone IS NOT NULL  //uguale

- BONUS 10 Selezionare tutti gli studenti il cui nome inizia per "E". 
> SELECT * FROM students WHERE name LIKE 'E%'  // https://www.w3schools.com/sql/sql_like.asp find any walue that start with 

- BONUS 11 Contare tutti gli insegnanti che iniziano con “E” (suggerimento: guardate l’operatore COUNT). 
> SELECT COUNT (*) FROM teachers WHERE name LIKE 'E%'; // conta tutti

- BONUS 12 Contare tutti gli insegnanti che non hanno un numero di telefono
> SELECT COUNT (*) FROM teachers WHERE phone IS NOT NULL  // nice
