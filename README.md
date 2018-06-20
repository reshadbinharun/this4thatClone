# Minerva ThisThat Pairings Clone
Md Reshad Bin Harun
Project Completed: June 29th, 2018

1. Requirements:
    1. The site looks visually distinct from the original, while retaining all functionality. When a "This" or "That" text div is clicked, or when the "Refresh" button is clicked, new pairings are asynchronously loaded to replace current pairings. As with the original site, clicking on "For" does not cause this change.
    2.  The same set of This/That pairings have been used as original site.
    3. JQuery has not been used. Libraries used on the client-side include Google Fonts.
2. Bonus Implementation:
    1. I used CSS, and HTML to design the front-end. Javascript functions were used to handle events and cause asynchronous changes.
    2. I implemented a back-end server written in Node.js with an API to return a "This/That" pairing to client. A Javascript function generates a GET request, and the pairing is returned as a JSON object which is then parsed to asynchronously edit text divs. The benefit of using an API call to a back-end server is that for a potentially larger list of pairings, a huge amount of data is not returned to the client machine. Having a much larger list of pairings to choose from will be feasible if the list is stored in the back-end server instead of on the client-side HTML. JavaScript's Math.Random() was used to randomly pick a This/That pairing.
    3. Additional Features:
        I thought it would be cool to have some features that could be personalized/randomized on the client-side too! The same javascript function that asynchronously alters the text divs for the This/That pairings also randomly pick 2 separate fonts, and 2 separate colors for the font, on each new click. This "flashy" color-font combination is one of the reasons I decided to keep the rest of the website's visual minimalist as I believe too much color can very easily seem overwhelming!
3. Submission Notes:
    1. Please find the .zip file attached in email submission.
    2. Instructions on setting up the project in '*nix' environment:
        a. install node package manager using "npm install"
        b. run the server using "node index.js" after once in root directory
        c. after the server is running, the app should be listening on PORT 3000 so make a GET request via a web browser with
        "http://localhost:3000/"
        d. I have also deployed the website on heroku, so the website should be live on: https://thisthatree.herokuapp.com/
4. Process for building clone:
* Made a use-case work flow: user clicks on div -> API call -> JSON object returned -> parsed to make asynchronous change on HTML
* Set up back-end server with routes to serve index page and to serve GET request for pairings
* Randomized pick of words from each list using JavaScript
* Made barebones client-side HTML to allow for asynchronous writing of HTML
* Included subsidiary features such as links to share work on twitter, and profiles links for original creators
* Implemented additional font/color change features
* Beautified front-end using CSS
* Deployed on Heroku so that website can be accessed from anywhere
