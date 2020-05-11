# AQ-WordPress-Test
Per lo sviluppo e l'installazione di wordpress è stato utilizzato Docker

## 1) Contenuto
Il repository è stato inizializzato nella cartella di progetto ed è stato configurato un punto di mount di tipo "bind" nella cartella wp-content per alleggerire lo stack e modificare agevolmente i file.

## 2) Child Theme
Il tema scelto è Customizr. Per la personalizzazione del tema e l'inizializzazione di un template custom è stato creato un child theme, inizializzato in:
```
wp-content
  -themes
    -customizr
    -customizr-child
```

## 3) Plugin
E' stato inizializzato un plugin vuoto in:
```
wp-content
  -plugins
    -meal-db
```

## 4) Esito
A causa di diversi errori nella valutazione del tempo a disposizione ed alcune lacune nel linguaggio PHP non mi è stato possibile procedere oltre con il test. L'idea sarebbe stata quella di definire una nuova action all'interno del file functions.php che, definiti i vari endpoint, eseguisse il fetch di "x" (definiti da alcune impostazioni del plugin personalizzato in una view admin) ricette da [MealDB](https://www.themealdb.com/api.php), visualizzate poi all'interno di un template customizzato ad-hoc per ricevere in maniera ordinata i risultati della call.
