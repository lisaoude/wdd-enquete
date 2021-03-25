# Minor WDD Enquête

_Made for Browser Technologies @ cmda-minor-web 2020 - 2021_

<!-- # Gifinder as a Progressive Web App

_Made for Progressive Web App [@ cmda-minor-web 2020 - 2021](https://github.com/cmda-minor-web)_

![Gifinder Mockups](https://user-images.githubusercontent.com/57795294/111635461-c7947800-87f7-11eb-94dc-198ce14e6aaa.png) -->

---

<!-------------------------- New Paragraph -------------------------->

## :pencil2: App description

<!-- Always wanted to quickly see the trending GIFs? **_Gifinder_** is here! On load, you will get 24 GIFs that meet your requirements!
By clicking on one of the GIFs, you will see that GIF's title, posted time, original source and a link to view the GIF at [Giphy.com](https://giphy.com)

Gifinder is a server side rendering application.

[**_My work_** can be viewed right here](https://gifinder-pwa.herokuapp.com/) -->

<br/>

<!-- I have also made a [Wiki](https://github.com/lisaoude/Gifinder/wiki), where I kept a weekly log, explained some things about map, filter & reduce and made some JavaScript related annotations.

<br/>  -->

---

<!-------------------------- New Paragraph -------------------------->

## :pushpin: Table of Contents

<!-- - [What does this Web App do?](#gem-What-does-this-Web-App-do?) -->

<!-- - [API](#link-API)
- [Used Packages](#gift-Used-Packages)
- [Install](#inbox_tray-Install)
- [Next Steps](#telescope-Next-Steps)
- [License](#closed_lock_with_key-License)
- [Sources](#books-Sources) -->

<br/>

---

<!-------------------------- New Paragraph -------------------------->

<!-- ## :gem: What does this Web App do?

- Fetch & show the trending GIFs on load
- Fetch & show the user GIFs based on the value they haved typed into the input field
- Fetch & show the user the details of a GIF they clicked on
- Provide the user with feedback while the content is loading
- Provide the user with feedback when hovering over a GIF

<br/>  -->

---

<!-------------------------- New Paragraph -------------------------->

<!-- ## :link: API

### :question: Which API did I use?

This Web App has been designed and developed with the [the Giphy API](https://developers.giphy.com/docs/api/).
Giphy has the largest GIF library in the world and their API makes it possible to seamlessly integrate these GIFs into any application.

<br/>

### :eyes: What can you do with this API?

_All information can also be found on [the Giphy website](https://giphy.com)_

- Return a random GIF
- Show trending GIFs to users
- Let the user search for GIFs, using a word or phrase
- Convert what the user typed into the input field into the perfect GIF using their :sparkles:special sauce:sparkles: algorithm
- Autocomplete user input with a list of valid terms that completes what the user has typed into the input field
- Generate a unique ID to assign to each new user in an application
- Generate one or multiple GIFs by ID endpoint
- Provide users with a list of GIF categories
- Provide users with a list of the trending search terms
- Suggest searches to users
- Upload content programmatically on Giphy.com -->

<br/>

<!-- ### :raising_hand: What did I do with this API?

I have implemented the following points into **_Gifinder_**:

**Home page**

- Show trending GIFs to users on load of the page

<br/>

**Detail page**

- Generate a GIF by ID endpoint -->

<br/>

<!-- ### :end: Endpoint & parameters -->
<!-- The API that was used is the API supplied by The Movie DB. These are public APIs and can be found at the link below:

https://developers.themoviedb.org/3/

This has been my 'standard' endpoint to which several parameters have been added to retrieve the data. The parameters below were used to obtain the various information:

discover/movie
movie/${movieID}
movie/${movieID}/recommendations
movie/${movieID}/watch/providers
search/movie
Based on these parameters, it can be seen that I show discovery movies, a specific movie, recommended movies based on a specific movie, the places where this specific movie can be viewed and the user can search for movies.

---
-->

<!-------------------------- New Paragraph -------------------------->

<!-- ## :open_file_folder: Folders & files

### Folder structure

During the development of Gifinder, I worked with modules for the first time. In my previous 'projects', as far as we can even call it that, my whopping 3 to 100 lines of JavaScript would just live in the same document. I used such little JavaScript, that it wasn't necessary to split it up at all. Because I'm obviously using MUCH more JavaScript for Gifinder, modules are great to keep everything organized. My folder & files structure for Gifinder looks like this:

![Folder & Files Structure](https://user-images.githubusercontent.com/57795294/109702534-a5aeba80-7b94-11eb-9be8-33a680f1eb2f.png)

<br/>

### Explanation folder structure

#### Assets

- Basically all code, except for my `index.html`, can be find inside this folder

<br/>

#### Scripts

- In here all my JavaScript code can be found

<br/>

#### Components

- In this folder, my folder with separate elements can be found, as well as my larger components, amde with those separate elements. In this folder my `index.js` file can also be found.

<br/>

#### Index.js

- Although this is a file and not a folder, it's definitely worth talking about. In this file I import all the separate elements made inside the `elements` folder. This way I can import these elements with way less code in my other files. An example can be found below.

##### **Example**

```js
// Messy, unnecessarily much code
import { elementOne } from "./file1.js";
import { elementTwo } from "./file2.js";
import { elementThree } from "./file3.js";
import { elementFour } from "./file4.js";
import { elementFive } from "./file5.js";
```

```js
// Clean, easily understandable code
import {
  elementOne
  elementTwo
  elementThree
  elementFour
  elementFive
  } from './index.js'
```

<br/>

#### Config

- In this folder, my `config.js` files can be found. In this file I export variables, such as the url and key I need for my API.

<br/>

#### Modules

- The `getData.js` file inside this folder does just what its name says: get the data. It fetches either the trending gifs on load, or fetches the gifs that the user has searched for using their input in to the input field.
- The `reloadHome.js` file inside this folder reloads the content on the home page after a request has been made. It makes sure to delete the previously loaded content before shaowing the new content.

<br/>

#### Routes

- The routes folder contains my ``router.js` file, where all possible routes are handled by the router. Because I use routie as my router, there's also a `routie.min.js` file. This file is provided for by Routie, and does not contain self-written code.

<br/>

#### Views

- The views folder contains all the pages that are rendered after a request has been made. These two pages use the imports from the `index.js` file in order to build all the HTML from scratch.

<br/>

#### States

- The states folder contains the loading state, which is shown during the loading of the gifs.

<br/>

#### Main.js

- This file is used to trigger the router and get Gifinder started.

<br/> 
-->

---


<!-------------------------- New Paragraph -------------------------->

<!-- ## :gift: Used packages

### :smiling_imp: nodemon
[Nodemon](https://www.npmjs.com/package/nodemon) is a tool that helps with the development of node.js based applications. The nodemon package restarts the node application automatically when any file changes are made inside the directory.

</br>

I installed nodemon to quickly see wether the changes I made caused any errors, and also for the convenience that comes with automatic restarts.

```
npm i -g nodemon
```

</br>

### :monorail: express
[Express](https://www.npmjs.com/package/nodemon) is a node.js framework. 

</br>

I installed express, because this package makes routing via the server easier. Another reason for installing express, was the support for many template engines, as I used one for this project, but hadn't decided on one just yet.

```
npm i express
```
```
const express = require('express');
```

</br>

### :memo: ejs
[Ejs](https://www.npmjs.com/package/ejs) is a template engine that makes it possible for JavaScript code to be injected into the client.

</br>

I installed ejs, because the package is easy to understand, has a gentle, gradual learning curve (which makes it great for newbies - like me!) and using the package makes it easier to inject dat from the server into the client.

```
npm i ejs
```
```
app.set('view engine', 'ejs');
```

</br>

### :large_blue_circle: dotenv
[Dotenv](https://www.npmjs.com/package/dotenv) is a package that loads variables from a ```.env``` file.

</br>

I installed dotenv, because it helps to store sensitive data (such as the API key), which can then be hidden from the GitHUb repository using my ```.gitignore``` file.

```
npm i dotenv
```
```
require('dotenv').config();
```

</br>

### :dog::soccer: node-fetch
[Node-fetch](https://www.npmjs.com/package/node-fetch) is a module which works just like the ```window.fetch``` methode does client side, but for the server side.

</br>

I installed node-fetch, because it allows me to do an API fetch via the server side.

```
npm i node-fetch
```
```
const fetch = require('node-fetch');
```

</br>

### :arrow_double_down: compression
[Compression](https://www.npmjs.com/package/compression) is node.js compression middleware. 

</br>

I installed compression, because it  ensures that JSON and other static file responses are smaller.


```
npm i compression
```
```
const compression = require('compression');
```
```
app.use(compression());
```

</br> -->


---

<!-------------------------- New Paragraph -------------------------->

<!-- ## :inbox_tray: Install

### 1. :dancers: Cone this repo

Before we can get started, we'll need to clone this repo.
This can be done by typing the following line of code into your terminal:

`git clone https://github.com/lisaoude/gifinder-pwa.git`

<br/>

### 2. :computer: Install package

Next, we will have to install the used packages.

`npm install `

<br/>

### 3. :arrow_forward: Start local dev environment

This can be done by typing the following line of code into your terminal:

`npm run dev`

<br/>

### 4. :european_post_office: Build export

Almost done! We just need to navigate to the localhost in the browser.

`npm run build`

<br/> -->

---

<!-------------------------- New Paragraph -------------------------->

<!-- ## :telescope: Next Steps

We all know creative developing projects are never _truly_ done..  
These are some next steps that I would love to make:

- [ ] Make it possible to let the users search for GIFs -->

<!-- - Make it possible for the user to save gifs, in the following ways:

  - Save the gifs to a favorites list
  - Save the gifs to a special collection, which the user can name themselves (e.g. funny gifs, cat gifs, etc.)
  - Save the gifs to their device (download)

- Give Gifinder a random mode

  - Returns a random GIF o the user after a button press

- Autocomplete user input with a list of valid terms that completes what the user has typed into the input field

- Provide users with a list of GIF categories
- Provide users with a list of the trending search terms
- Suggest searches to users -->

<br/>

---

<!-------------------------- New Paragraph -------------------------->

## :closed_lock_with_key: License

This repository is licensed as [MIT](https://github.com/lisaoude/browser-technologies-2021/blob/master/LICENSE) by © Lisa Oude Elferink, 2021

<br/>

---

<!-------------------------- New Paragraph -------------------------->

## :books: Sources

<!-- - Schepenaar, W. (2018, June 12). Server-side vs Client-side Routing. Retrieved March 8, 2021, from [Medium](https://medium.com/@wilbo/server-side-vs-client-side-routing-71d710e9227f)
- Ian Schoonover. (2020, June 27). How to Install Node JS on Windows 10. Retrieved March 8, 2021, from [YouTube](https://www.youtube.com/watch?v=AuCuHvgOeBY)
- Installing Express. (2021). Retrieved March 8, 2021, from [Expressjs.com](http://expressjs.com/en/starter/installing.html)
- The Net Ninja. (2020).  Node.js Crash Course Tutorial. Retrieved March 8, 2021, from [YouTube](https://www.youtube.com/playlist?list=PL4cUxeGkcC9jsz4LDYc6kv3ymONOKxwBU)
- npm: ejs. (2021, February 6). Retrieved March 9, 2021, from [NPMjs.com](https://www.npmjs.com/package/ejs)
- npm: nodemon. (2021, January 6). Retrieved March 23, 2021, from [NPMjs.com](https://www.npmjs.com/package/nodemon)
- npm: dotenv. (2019, October 16). Retrieved March 16, 2021, from [NPMjs.com](https://www.npmjs.com/package/dotenv)
- npm: node-fetch. (2020, September 5). Retrieved March 16, 2021, from [NPMjs.com](https://www.npmjs.com/package/node-fetch)
- The Net Ninja. (2019). PWA Tutorial for Beginners. Retrieved March 22, 2021, from [YouTube](https://www.youtube.com/playlist?list=PL4cUxeGkcC9gTxqJBcDmoi5Q2pzDusSL7)
- npm: compression. (2019, March 18). Retrieved March 23, 2021, from [NPMjs.com](https://www.npmjs.com/package/compression) -->



<!-- In this course we will convert the client side web application previously made Web App From Scratch into a server side rendered application. We also add functionalities based on the Service Worker and turn the application into a Progressive Web App. Ultimately we are going to implement a series of optimisations to improve the performance of the application.

## Learning goals
- _You understand the difference between client side and server side rendering and you can apply server side rendering
in your application_
- _You understand how a Service Worker works and you can implement it in your application._
- _You understand how the critical render path works and how you can optimize it for a better runtime and / or perceived performance._

[Rubric with learning goals](https://icthva.sharepoint.com/:x:/r/sites/FDMCI_EDU__CMD20_21_Minor_Web_5i7j73jt/_layouts/15/Doc.aspx?sourcedoc=%7B276F53A7-2531-4006-8AD2-08C9A82D3A11%7D&file=PWA%202021%20Rubric.xlsx&action=edit&mobileredirect=true&wdPreviousSession=92686bea-446f-40e3-9303-33fa3f832b82&wdOrigin=TEAMS-ELECTRON.teams.undefined)
