# SEI Project 2: NewsApp

## Overview
My partner and I built a React app within 48 hours like a hackathon style project. We pair-coded throughout the project, taking turns to write the code or to provide support. We did this over zoom and VS Code’s live share feature allowing us to work simultaneously on this project. We agreed to build a NewsApp using the Guardian API to show the user the latest news stories. Our project contained good functionality allowing the user to search for topics they are interested in and save news articles to be retrieved again to read. 

<div align="center">
<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924208/Screenshot_2021-09-19_at_16.21.10_ipksps.png" width="800px" />

<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924236/Screenshot_2021-09-19_at_16.21.31_xx91c4.png" width="800px" />

<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924234/Screenshot_2021-09-19_at_16.21.47_aiusnv.png" width="800px" />
</div>


## Brief
Using an external API create an app with multiple components, a router and several pages. The app should be created using JavaScript, React and HTML/CSS for styling.

## Deployment 
https://ayamallahx-newsapp.netlify.app

## Timeframe
48 hours

## Technologies
* HTML
* CSS
* SASS
* Bulma
* JavaScript
* React
* Axios

## Installation
* Clone or download the repo.
* Install all frontend packages (from package.json) by running the command `yarn`.
* Start server with `yarn start`.

## Plan
We both wanted to create an informative app with a clean design and clear UI. We chose a grey and aqua as our colour pallet and a minimalistic look to the design. We chose to use Bulma and CSS to style the app, this gave us flexibility to style elements effectively, when Bulma was not needed.  

<div align="center">
<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924221/d61nHqLT8zETOEvTY38VMpya7tlEbbtSHoMfRMCKSgpahbDJblhoDCTKIGEH62vlCWkfG33Qbi2uGhof_Pwe3tcTfTrlsaX_X3vV1Z8Bxb0DGfMBLhzXJet26rUBzs2oXMF97RCD_s0_d8pgo6.png" width="550px" height="350px"/>  
</div>

## Approach

My partner and I chose to paircode the whole app together via Zoom, we took turns to code, while using the live share feature in VScode so we could see what changes were being made. We started outlining our MVP as we only had 48 hours to complete this app. Using the Guardian’s API we displayed news articles on an index page. The user is able to search for topics that interest them. They can click a news article and it will display further detailed information, also allowing the user to access the story on the Guardian’s own website.

<h4>Making a specific article GET request:</h4>
To display a detailed version of each article, we would make a get request for that specific article. After reading through the API documentation, we realised that it is possible to use the ID from each article for the GET request to achieve this. To get the ID we included the ID in the URL of the specific article, so that when the user navigated to the news story, the ID was accessible in the URL pulling all the relevant information.

<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924220/S50ETHflm1aprkLMxf0pOV1t5v_CLq3S99gMQMirvTCYMcWm4OCqoOQ18xZi4g87n7IQZvwTCuTXi2X818_jnL_tHZzVL-tXz_Ixb76LmUH5p165rBX4knq90gZEWyvqWNsikB8w_s0_ig4abw.png" width="500px" />

<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924229/cu1B6t8Yn0VAL2UTFTewDb-TaldWVCaN7XQ9pSzz5VneXmMXo15UPAzRL1MhSBtn7nMWCTwmg71Iw-tBSOr6oTwUtqlugjF1V1rgcqakCcwL1PBvkl7q-j9P5SiJVWIpWG0vpNrK_s0_vo1gh1.png" />

<h4>Displaying all articles on the index page:</h4>
Initially we used a basic request to the API to display all articles held in the API, however after reading further into the documentation and adding our search input functionality. We found a way of using a search function in the request, meaning we could use one useEffect to display results from a search using a new GET request from the API otherwise remain displaying all the ‘Top Headlines’.

<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924239/tkFs3tc2aR84BT-AN4ZBqYeXTM_e6cSAkdXPpRhIomoIepIwg-Qo1jVRDdyj3OcOTvlnj5CwSHOXQ73pPIVKSDi-hCoFgZBn9PW0gjFGHYesZoWVIfoQx4KGPuzXqOktWKCyQbdN_s0_ab90zd.png" />

After we managed to complete our MVP, we decided to start with our Nice-To-Haves. The main extra feature we wanted was the saving feature allowing the user to save their favourite news stories to be read at a later date. Once the user clicks on the ‘save’ button the article information is set to state and then saved to local storage allowing access to that data whenever on the ‘My News’ page.

<img src="https://res.cloudinary.com/dhrxw6zhp/image/upload/v1632924243/em2qBWg25IDGoy-ARXMWq6oHRkjXZTUHrWffcSIyXJY7dLV7w3NmjZt97fJkIvJS5Wc1YQ11zEYbZrNgB_xQ4LZqsogcpvR1zdmWhecJNF1RMNEIW9v1AEt0RtbnMfK808zeMgAO_s0_vc3k43.png" width="500px"/>

We made sure to allow time for polishing and styling which was led by me. I went for a simple classy look which turned out to be quite similar to our first wireframe but the finished result was very smooth.


## Wins 
This was my first pair coded project. I really enjoyed it and took advantage of working with someone else, exploring different coding styles and collaboratively problem solving.  

A massive win for me in this project was the use of local storage for the save feature for each article. I had to research and understand how the local storage works. The user can search for topics they are interested in and save news articles to be retrieved again to read.

Another win would be creating an aesthetically pleasing and responsive app together. It was important that the site would be functional and look good when displayed on any device.  

## Challenges
One of the biggest challenges during this project was understanding the API. It was hard at first to figure out how the IDs of the articles were being displayed, which made it hard at first to view one single article.  

Understanding and navigating the API. We spent some time reading the documentation provided by the API’s website and testing the requests in Insomnia. Once we managed to do so it was a big win for us.  

## Bugs
The first bug I noticed was when an article that is displayed doesn't have a thumbnail attached in the API, it will display a broken image link. This does not look nice and makes the user experience less professional. A possible solution would be to filter out any news stories that do not have an image and not display these at all. 

As the timeframe we had was short we were not able to fix all the problems we had. For example when testing out the save feature, we realised that each time a user saves an article it overwrites the current article in local storage. 

## Future Improvements
* Fix the save feature for articles, so that a user can save more than one article when logged in.

* I also want to be able to add categories e.g. sport and health, for the user to be able to filter out what articles they would like to read.

* Add more styling, as most of the styling was done by myself really quickly, I would like to spend more time making it stand out.

