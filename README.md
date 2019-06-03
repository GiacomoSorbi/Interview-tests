# Interview tests

## General description:

These interviews are meant to test a candidate suitability to work in a team, pick priorities, manage pressure and optimise the outcome under time constraints.

The interviews are supposed to be assisted and recorded by an interviewer.

The candidate can use whatever library, framework or other tool he/she considers appropriate for the job, as long as proper motivation and support can be given for each choice (ie: using `create-react-app` to quickly get a lot of boilerplate code set up and running is fine; importing every package of `BootStrap` just to style a single button might not be fine).

Maintainability and quality of code need to be stressed as important even if it is a quick demo.

The candidates is not expected to produce a complete product; on the contrary, building a non-working app, but also implementing plenty of testing and most of the business logic by the end of the test is a fine behaviour, as it might be focusing on the UI and using mostly mock-data.

The candidate is expected to spend 5-10 minutes to learn the basic ropes of any given API and must be made aware that he/she can ask the interviewer further clarification or instructions at any time - some tasks are given as vague on purpose, just to assess how much the candidate is actually rationally interpreting the specs and not merely following them in a drone-like mindest.

All the scenarios are to be considered [kobayashi maru](https://en.wikipedia.org/wiki/Kobayashi_Maru)-like, ie: losing scenarios meant to push the candidate to choose among different sub-tasks as deliverables. The candidate must not be made openly aware that completion is not important, though; furthermore, a particularly fast and skilled candidate that was to approach the completion with most of the test running and properly structured, can be given a few extra sub-tasks or asked theoretical questions about the choices he made and their trade offs.

The user is going to be given only the first part of the test description - the part about extra questions is to be administered according to his/her own performance during the test itself, without any forenotice.

## Front-End (React):

### Weather API

Create a weather app that allows me to query for a specific city and obtain either [its currente weather](https://openweathermap.org/current) or [the forecast for the next 5 days](https://openweathermap.org/forecast5). It is important to recommend the user to register to the service ASAP, as the activation of the account can take a few minutes; emphasis need to be put also on displaying the results.

*Question about disambiguating location and handling errors.*

### XKCD comics viewer

Create a comic reader app that opens with the last comic, using [their public API](https://xkcd.com/json.html); the app should also include a last and a next button (both disabled when the last comic is actually visualised), a random comic button, a previous and first comic (both disabled when the first is actually visualised).

*Questions about loading, pre-fecthing and optimising image formats can be formulated during the administration of this test.*

### Top Rated TV Series

Create an app to list the top rated TV series according to [MovieDB and its API](https://developers.themoviedb.org/3/getting-started/introduction), displaying each of them in a simple tv show-card that can give me more details either on click or on hover.

*Questions about pre-fecthing and paginations.*

### Domain Lookup for availability with Common Extensions

Create an app to check if a given domain is already registered with the common extensions (`.com`, `.net`, `.org`, etc...) using [this API](https://www.who-hosts-this.com/Documentation).

*Question on how to implement something closer to [Domize](https://domize.com/), debouncing, optimising UX, caching results.*

### Technologies Inspector on listed domain

Create an app that allows the user to generate a list of domains to be queries (with proper insertion and removal of each item) and then runs a check of all of them using [this API](https://www.who-hosts-this.com/Documentation) (scroll down up to "Technology detection") and then displays the data according to the results.

*Questions about how to make the removal more efficient (like using `data-` or `id` parameter to just remove the `event.currentTarget`, instead of generating a removal function for each item), grouping results by same technology, displaying them with responsiveness and/or sortability.*
