FEATURE 2: SHOW/HIDE AN EVENT'S DETAILS
    Scenario 1: An event element is collapsed by default
        Given the user has not clicked the event element yet.
        When the user clicks the element
        Then the event details collapse
    Scenario 2: User can expand an event to see its details
        Given the user needs/wants details from an event
        When the user clicks on an event
        Then details of the event expands
    Scenario 3: User can collapse an event to hide its details
        Given user no longer needs/wants the event details
        When user clicks on the expanded event details
        Then the event details collapse
FEATURE 3: SPECIFY NUMBER OF EVENTS
    Scenario 1: When user hasn’t specified a number, 32 is the default number
        Given the user did not specify the number of events, the default number is 32
        When user begins searching events
        Then user will get 32 events listed
    Scenario 2: User can change the number of events they want to see
        Given the user specifies the number of events
        When user searches for the specified number of events
        Then the user will get the number of events from the chosen number amount.
FEATURE 4: USE THE APP WHEN OFFLINE
    Scenario 1: Show cached data when there’s no internet connection
        Given the user is not using the internet and wants to use application
        When user uses app offline
        Then user can use all cached data in application
    Scenario 2: Show error when user changes the settings (city, time range)
        Given the user tries to change settings in the application
        When user tries to change settings
        Then the user will get an error message on the application
FEATURE 5: DATA VISUALIZATION
    Scenario 1: Show a chart with the number of upcoming events in each city
        User wants/needs to see a chart of upcoming events
        When user clicks on chart
        Then user will be given a chart with all upcoming events
