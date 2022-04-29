# db-sql-1

- studio delle slide
- recupero della registrazione video per assenza

- selezionare tutti gli insegnanti
> SELECT * FROM teachers; //ossia seleziona ogni valore in colonna teachers

- seleziona tutti i capi di ogni dipartimento
> SELECT head_of_department FROM department // same

- selezionare tutti i corsi di laurea magistrae
> SELECT * FROM degrees WHERE level = 'magistrale'  // prende solo ('), non (")

- slezionare tutti gli studenti che hanno come nome Marco
> SELECT * FROM students WHERE name ='Marco' //stesso principio
