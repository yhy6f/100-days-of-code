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

### Day 13: Feb 2, 2022, Wednesday

**Today's Progress**: Geocoded the locations of the results returned from API call, added markers based on the locations, and added animation effects of markers dropping.

**Thoughts**: Finally figured out that to use the Geocoder class, you need to do new google.maps.Geocoder(), just like map = new google.maps.Map(). It wasn't clear in the Geocoder API documentation, but it would have easier to make the connection for more experienced programmers I think. I'm still glad I figured it out although it took some time. Also, [This Youtube tutorial](https://www.youtube.com/watch?v=tmdtH1hwlDo) on Google Maps markers was clear, concise and useful. I appreciate the author's work.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 14: Feb 3, 2022, Thursday

**Today's Progress**: Added info window to each marker in pet finder app.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 15: Feb 4, 2022, Friday

**Today's Progress**: Changed marker event listenr and handler so that info window disappear after other info windows are clicked.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 16: Feb 5, 2022, Saturday

**Today's Progress**: worked on portfolio website

**Thoughts**: I achieved the behavorial goal (per the book Procrastination) of spending 4 hours, but the progress was not as much as I had expected compared to the time I spent. Wasted some time going back and forth on some decisions. Need to overcome my perfectionalism!

**Link(s) to work**
1. [my Github.io repo](https://github.com/yhy6f/yhy6f.github.io)

### Day 17: Feb 6, 2022, Sunday

**Today's Progress**: Added more clips to the portfolio website

**Link(s) to work**
1. [my Github.io repo](https://github.com/yhy6f/yhy6f.github.io)

### Day 18: Feb 7, 2022, Monday

**Today's Progress**: Fixed an issue in pet finder app: previously when a shelter doesn't have photos in data returned by API, the marker would not load. Fixed the issue by adding a condition to the code that generate the JSX string passed into setContent() method. Also moved the JSX code into a separate function.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 19: Feb 8, 2022 Tuesday

**Today's Progress**: Tried to look for a solution to add google API key as environment variable for the pet finder app. Converted the code to an express app, although it didn't solve the problem. 

Also attempted to add a refreshToken function that does the samething as the curl request referred in API document to refresh access token, which is required to make Petfinder API calls. 

```
curl -d "grant_type=client_credentials&client_id={CLIENT-ID}&client_secret={CLIENT-SECRET}" https://api.petfinder.com/v2/oauth2/token
```

**Link(s) to work**
1. [my github repo: pet_finder express app](https://github.com/yhy6f/petfinder-express-app)

### Day 20: Feb 9, 2022 Wednesday

**Today's Progress**: Found a solution to not push Google API key to Github: store the key in an environment.js file and uses document.createElement("script") and append to the body of html file.

**Thoughts**: After pushing the code I realized I still included my google api key in my old script tag code that was commented-out. So I had to delete that commit from github and locally. Thankfully found a very useful stackoverflow [post](https://stackoverflow.com/questions/448919/how-can-i-remove-a-commit-on-github). After following the instructions (git rebase -i HEAD~2, git push origin +branchName --force), the local repo was reverted to what it was before the commit in question, and I added back the code.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 21: Feb 10, 2022 Thursday

**Today's Progress**: Worked on the refreshToken function in token.js that would refresh the access token. Although still not able to return the token value and assign it to a variable in script.js.

**Thoughts**: My engineering friend gave me some hints: -d will send the data given to it as the body of a POST request, whereas my previous attempt was placing the data in the headers of a GET request: fetch("https://api.petfinder.com/v2/oauth2/token",options)

So to make the -d request, we'd have to switch the method to "POST", create a body object, convert the body into a string using JSON.stringify() because bodies of HTTP request must be strings. 
```
const body = {
    "grant_type": "client_credentials",
    "client_id": "...",
    "client_secret": "..."
}
fetch('https://api.petfinder.com/v2/oauth2/token', {
        method: 'POST',
        body: JSON.stringify(body),
        headers: {
            'Content-Type': 'application/json; charset=utf-8'
        }
    })
    .then(response => response.json())
    .then(auth => {return auth.access_token})
    .catch(error => console.log(error)

```
But still wasn't able to return the value of auth.access_token and assign it to a variable.

**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 22: Feb 11, 2022 Friday
**Today's Progress**: Continued to work on the refreshToken() function for pet finder app. Also tried to deploy the pet finder app on Heroku but the map didn't render.
**Thoughts**: hint from my JavaScript course instructor: adding let access_token = '' inside the refreshToken() function and in the last .then() of the fetch request, add access_token = auth.access_token, and add return access_token after the fetch request. The function returns an empty string because the return runs before the fetch is executed, and he suggested I should turn this into an async function. I tweaked this function a few different ways but still didn't work. I should look closely into async and await.
**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 23: Feb 12, 2022 Saturdey
**Today's Progress**: Tweaked the css of the pet finder app so the search area is in the center of the page. Also updated the intro section of portfolio website and re-reorganized clips.
**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)
2. [my github repo: yhy6f.github.io](https://github.com/yhy6f/yhy6f.github.io)

### Day 24: Feb 13, 2022 Sunday
**Today's Progress**: Portfolio website: finalized bio section in header; added clips and headerimages; added target="_blank" to all a tags; added hyperlink to skills section so a click takes user to corresponding clips; added dotted line under all hyperlinks.
**Link(s) to work**
1. [my github repo: yhy6f.github.io](https://github.com/yhy6f/yhy6f.github.io)

### Day 25: Feb 14, 2022 Monday
**Today's Progress**: Made the refreshToken function work, with some help from my friend.
**Thoughts**: Turns out, to return value from a fetch request, you need to return the promise in the function and access the value in .then() outside of the function, per this [stackOverflow post](https://stackoverflow.com/questions/47604040/how-to-get-data-returned-from-fetch-promise).
**Link(s) to work**
1. [my github repo: pet_finder](https://github.com/yhy6f/pet_finder)

### Day 26: Feb 15, 2022 Tuesday
**Today's Progress**: Portfolio website: re-ordered some sections, small tweaks
**Thoughts**: .
**Link(s) to work**
1. [my github repo: yhy6f.github.io](https://github.com/yhy6f/yhy6f.github.io)


### Day 27: Feb 16, 2022 Wednesday
**Today's Progress**: Added typewriter animation to my titles in the portfolio website, with typing and deleting effect.
**Thoughts**: It took me a while to find the right keyword to search, but eventually I found a [tutorial](https://usefulangle.com/post/75/typing-effect-animation-javascript-css) and was able to insert the javascript. It took a few trial and errors to get the css right for the style of my website. The example code from the tutorial puts the content of the text added or deleted inside a div with id of #text, and set the color and size for #text in css. To conform to the style of my website, I made that a p tag, because p tags in the header has style set up in the css file of the web template. Another thing was, when I just copied and pasted the css for #container, the title and bio section would flicker, because when all the words are deleted, the div becomes empty, and I figured that was causing the height of the div to change. So the solution was to set a fixed height for the #container div.
**Link(s) to work**
1. [my github repo: yhy6f.github.io](https://github.com/yhy6f/yhy6f.github.io)

