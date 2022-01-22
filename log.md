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

### Day 4: January 19, 2022, Wednesday

**Today's Progress**: None. Taking a break as I didn't feel very well.

**Thoughts**: Guilty but not guilty.

### Day 5: January 20, 2022, Thursday

**Today's Progress**: Tweaked the html file. Connected the user input of a distance, the click to search button and the API endpoint. For next step I'd like to incorporate the user location into the API endpoint, and render the map centered around the user location in the page. So basically incorporate the first part of the googlemap tutorial into this app, and make the api endpoint responsive to an input.

I tried to get rid of the .DS_Store file by adding .DS_Store in gitignore, but it didn't work. Then I learned that you'd have to remove it (because it was already added) using `git rm --cached .DS_Store` and then git will start to untrack the .DS_Store file going forward.

**Thoughts**: Again, baby steps but making progress :)

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 6: January 22, 2022, Friday

**Today's Progress**: Started seeing CORS error when I tried to fetch data from the petfinder API endpoint, even though the same code worked yesterday. Since I wasn't able to fix the error despite trying what my JS instructor taught, I switched gear to add the map in first. I was able to console.log browser location and the API endpoint URL which is based on that location. To prepare for rendering the shelters as markers, I looked up the google maps [markers documentation](https://developers.google.com/maps/documentation/javascript/markers) to see what arguments it takes, specifically what should be passed into position. `position: myLatLng`, myLatLng should be an object: { lat: -25.363, lng: 131.044 }.

I learned that to make your local repo the same as the remote master branch, can be done with `git fetch --all`, and `git reset --hard origin/master`. [stackoverflow](https://stackoverflow.com/questions/1125968/how-do-i-force-git-pull-to-overwrite-local-files)

**Thoughts**: A bit frustrated about the CORS error. But glad got other things done that doesn't require using the petfinder API.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)
