# Events

    GET leagues/:id/events

## Description
Returns a list of Event objects for the league.

## Parameters
* id (required) - the League ID
* status - one of 'upcoming','ongoing','finished', 'postponed', 'interrupted', 'all'(default)
* fromDate - filters out events after a specific date, Date in short format
* toDate - filters out events before a specific date, Date in short format
* limit - Limits the number of events, positive integer
* offset - Used to iterate over a large number of items, integer
* teams - a comma-separated list of one or many team IDs for which you want to filter the events. For example, if you only want the events for a specific team. 
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esEvents'

## Return format
An object with the following keys and values:
* credits - a Credit object
* events - a list of Event objects