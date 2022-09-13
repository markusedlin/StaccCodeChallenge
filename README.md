# Stacc code challenge 2021

## Oppgavebeskrivelse
* I have chosen task a) where I must retrieve information from an API and display it in a simple web app.
* It retrieves all data and displays it below the search bar
    - I decided that it is not my task to decide which data fields should be displayed, but these can easily be changed.

## Hvordan kjøre prosjektet
    * make sure directory is \myapp
    * Enter in terminal: npm start
    -> should open browser with correct local host and port
## Hvordan ende prosjektet


How it works:
    * Enter a name or beginning of a name and click search
    * Loading 'animation' pops up and then disappears on result
    * Can enter a new name to change the KYC search.

## Kommentarer
- What I would like to add:
    * autocomplete for when typing a name
    * table within the return function(isn't as trivial as expected with react)
        - would look much cleaner
    * event listener for input so 'Enter' == search button click
    * get picture of person with some sort of wiki lookup
        - problem here is that it may not be the correct person
    * search icon instead of text 'Search'
    * Perhaps add a way to clear the data and 'table' without refreshing
    * Comparison button to be able to compare more than one person at a time (display 2 PEP at once)
    * Country code translator, from 'no' to 'Norway'
        - I found a table online for this and now have extracted necessary values. Wouldn't take extremely long to get this to work, but it is an extra step.

- Issues:
    * Gap between Alias and first seen if the person doesn't have more than one alias
    * Huge node_modules folder containing lots of files, not knowing how many of them are necessary. I'm not super familiar with this, and have decided to keep it.

- Struggled with:
    * Setting it up within only an html file after already setting it up through a node localhost, so I stuck with the npm method
    * React useEffect - having the get method within the useEffect based on an onChange input value.
        - Challening because when the initial render occurs, it tries to 'get' nothing which logs an error
            - (does it matter if it logs an error? as long as it doesn't show anything on the screen.)