# Date Suggest [WIP]

Because clicking on calendar widgets is so 90s.

# Idea

Create a script that returns ranked date suggestions from input string based on clever approximations:

# Samples

Input: `7 de 18`

Output:

1. December 7th 2018
2. 18th December 2008

Input: `ap 20 89`

Output:

1. 20th April 1989 ( explained: 1989 is closer year to today's date )
2. 20th April 2089

Input: `ju 20 12PM`

Output:

1. June 20th, current year, 12.00PM
2. July 20th, current year, 12.00PM

Input: `tom 3`

Output:

1. One day from now, 3PM
2. One day from now, 3AM

Input: `tom 11`

Output:

1. One day from now, 11AM (now AM shows first because 11AM is in working hours)
2. One day from now, 11PM


## Keywords to cover:

- month names (eg. a => april, j => june, july, d => december, n => november)
- today, tod
- tomorrow, tmrw
- yesterday
- am, pm and regex for 12a, 12p
- time: 12AM, 12.30PM, 12:30AM

(list not in particular order)


# Configuration

allow to configure behavior of the ranking engine
eg. if birthdate should behave differently, and should show past dates, if event
then show future dates, allow timeframes (eg. from-to dates to be suggested only)

