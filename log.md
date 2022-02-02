# 100 Days Of Code - Log

### Day 1: January 16, 2022, Sunday

**Today's Progress**: I followed along part I of this [Google Maps API tutorial](https://www.youtube.com/watch?v=C6VxJoR3754), which was about rendering a Google map based on user's location via navigator.geolocation.

**Thoughts** I've recently started (re)learning Javascript, and I'm working toward a project that would render Google Map on the page. I shopped around on Youtube for tutorials and was glad I found this one, newer and shorter. Before I was able to follow along the tutorial, I had to sign up for the Google Maps API key. I was frustrated and confused because it required me to hop around a few different places - but eventually I got my key. I followed along the instructions and got a map to render

**Link(s) to work**
1. [my github repo: googlemap](https://github.com/yhy6f/googlemap)

### Day 2: January 17, 2022, Monday

**Today's Progress**: I followed along part II of this [Google Maps API tutorial](https://www.youtube.com/watch?v=C6VxJoR3754) on the  Places API, which allows users to type names of places and autocomplete their search.

**Thoughts** It was cool to see it work. A few small hickups were all because of typos. Need to be careful when typing next time! A few things that I'd like to improve on: making the map div height and width responsive to window size; and move the map view center to newly added marker.

**Link(s) to work**
1. [my github repo: googlemap](https://github.com/yhy6f/googlemap)


### Day 3: January 18, 2022, Tuesday

**Today's Progress**: I made a basic UI for my pet adoption project with an input form. I tested out the petfinder API with curl, and tested out the endpoint URL using fetch(), and console.log the data I got back. I learned that you pass in the authorization token in a headers object into the second argument of fetch(), and that the humongous authorization token can be actually decoded using [this site](https://jwt.io/). Next step is to tie the input with the endpoint URL together.

**Thoughts** Felt good that I made steady progress, even these are baby steps.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 4: January 20, 2022, Thursday

**Today's Progress**: Tweaked the html file. Connected the user input of a distance, the click to search button and the API endpoint. For next step I'd like to incorporate the user location into the API endpoint, and render the map centered around the user location in the page. So basically incorporate the first part of the googlemap tutorial into this app, and make the api endpoint responsive to an input.

I tried to get rid of the .DS_Store file by adding .DS_Store in gitignore, but it didn't work. Then I learned that you'd have to remove it (because it was already added) using `git rm --cached .DS_Store` and then git will start to untrack the .DS_Store file going forward.

**Thoughts**: Again, baby steps but making progress :)

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 5: January 21, 2022, Friday

**Today's Progress**: Started seeing CORS error when I tried to fetch data from the petfinder API endpoint, even though the same code worked yesterday. Since I wasn't able to fix the error despite trying what my JS instructor taught, I switched gear to add the map in first. I was able to console.log browser location and the API endpoint URL which is based on that location. To prepare for rendering the shelters as markers, I looked up the google maps [markers documentation](https://developers.google.com/maps/documentation/javascript/markers) to see what arguments it takes, specifically what should be passed into position. `position: myLatLng`, myLatLng should be an object: { lat: -25.363, lng: 131.044 }.

I learned that to make your local repo the same as the remote master branch, can be done with `git fetch --all`, and `git reset --hard origin/master`. [stackoverflow](https://stackoverflow.com/questions/1125968/how-do-i-force-git-pull-to-overwrite-local-files)

**Thoughts**: A bit frustrated about the CORS error. But glad got other things done that doesn't require using the petfinder API.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 6: January 22, 2022, Saturday

**Today's Progress**: worked on javascript class project which is a news feeder app which uses News API, Guardian API and reddit data.

**Link(s) to work**
1. [my General Assembly git enterprise repo: feedr-app](https://git.generalassemb.ly/jasmineyehan/12-feedr-app/tree/master/feedr-starter-code)

### Day 7: January 24, 2022, Monday

**Today's Progress**: retested the pet finder app CORS error just to be sure. Didn't make much progress

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 8: January 27, 2022, Thursday

**Today's Progress**: Followed along Javascript course instructions on how to use Firebase API to build a forum page with realtime database of messages with CRUD functionalities (Create, Read, Update, Delete). (This wouldn't strictly qualify for the 100 days of code challenge, but since I'm still learning, I will give myself a pass on this)

**Thoughts**: The class was pretty dense and covered a lot of grounds. I had to get over the weird feeling of seeing new methods and using them in ways never seen before because they were specific to Firebase. 

**Link(s) to work**
1. [my General Assembly git enterprise repo: CRUD and Firebase](https://git.generalassemb.ly/jsr113021/16-intro-to-crud-and-firebase)

### Day 9: January 28, 2022, Friday

**Today's Progress**: Worked on the news feedr app. Made the page load the News API results once opened using window.onload(). Added search feature wherea a text input field pops up once the search icon is clicked on (by adding an active class) and passes the user input in that field onto the search endpoint of News API.

**Link(s) to work**
1. [my General Assembly git enterprise repo: feedr-app](https://git.generalassemb.ly/jasmineyehan/12-feedr-app/tree/master/feedr-starter-code)

### Day 10: January 29, 2022, Saturday

**Today's Progress**: Pet finder project: Incorporated the code I wrote days ago that return results based on lattitude and longitude into existing code. But I ran into a 400 error.

**Thoughts**: The CORS error on the pet finder app somehow disappeared after the herokuapp url was removed from the endpoint string. Very confused because when the code didn't have that url, there was CORS error as well. When I made the endpoint based on lattitude and longitude (as opposed to location=20740), the endpoint returned data in curl test but a 400 error in browser. 400 error means syntax error so it's quite confusing how this could happen.

**Link(s) to work**
1. [my General Assembly git enterprise repo: feedr-app](https://git.generalassemb.ly/jasmineyehan/12-feedr-app/tree/master/feedr-starter-code)

### Day 11: January 30, 2022, Sunday

**Today's Progress**: Worked on my personal portfolio website. Started off with a template and changed out some of the placeholder texts. Also researched how to add gifs.

**Thoughts**: Wanted to add gifs of screenshots of interaction with some of my past interactive graphics as examples of projects. Added a random exaple for testing and realized that I need to pay attention to the dimension of the gifs otherwise it'd messup the grid of the images.

**Link(s) to work**
1. [my Github.io repo](https://github.com/yhy6f/yhy6f.github.io)

### Day 12: Feb 1, 2022, Tuesday

**Today's Progress**: Attemped to add geocoding function to the petfinder app. Worked through the [geocoding documentation](https://developers.google.com/maps/documentation/javascript/geocoding)

**Thoughts**: At first was confused that it was another library that needed to be imported so added "geocode" & "geocoder" after "libraries=" in the string. Then read documentation more closely and realized that Geocoder is a class provided by the Maps JavaScript API. But using google.maps.Geocoder.geocode(...) returned error saying this is not a function. 

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)