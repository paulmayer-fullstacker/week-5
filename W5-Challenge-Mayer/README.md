# Finish the Weather Dashboard

## Introduction:

Herewith my submission for Week-5's challenge: an interactive weather app. The solution is a team effort, developed by Wizards of the Apocalypse.  

The solution comprises: a HTML index page (index.html), a CSS style sheet (style.css), and a Java Script (JS) file (script.js).

The HTML page is sparce, acting only as the entry point for the solution. Bootstrap styling is employed directly (in line), within the HTML, per Bootstrap best practices. The CSS style sheet offers sufficient additional styling. The JS file defines the functionality of the solution.

Specific solution features are not listed within this document. However, some justification of my solution strategy and JS coding will be offered.
The solution has been pushed to my GitHub repository and published to GitHub Pages, for public access and review.

---

## The Solution

### Behind the Weather Dashboard:

The main functionality of the interactive weather dashboard is defined within the JS file. The JS file contains the client-side logic, accommodating manipulation of the Document Object Model (DOM), and event handling. The JS file also manages API consumption and remote data access.   

The dashboard weather display relies on retreival of weather data from an Open Weather Map server. Here is the API call (provided by 8-UP), to the OpenWeatherMap API to retrieve current weather data. The call requires the location for the requested weather information (longditude and latitude) and an API key (also provided by 8-UP).  

    `https://api.openweathermap.org/data/2.5/weather?lat=${latitude}&lon=${longitude}&appid=${API_KEY}&units=metric`

The API call returnes a data object (JSON format) populated with current weather and some local data for the specified latitude and longitude. Before JS coding commenced, for the clinet-side script, the API call was tested using the REST Client extension for VSCode, published by Huachao Mao.

The JS file was judiciously commented, during development. However, during team collaboration exercises, most of the comments were removed. The HTML and CSS files still contain useful comments.  

### Collaboration:

Wizards of the Apocalypse started with a Minimal Viable Product (MVP), developing a usable product from there. The development project offered a very valuable exercise in collaborative development. Wizards of the Apocalypse spent relatively little time in development. Most contact time was spent practicing with GitHub.

### Development of the MVP

Development of the MVP took the form of Bug Fixing. Identifying issues with functionallity of the MVP, prioritising those issues, and allocating non-conflicting work to team members. In this way a flow of incrementally improved code was continually merged into GitHub. One of the tasks allocated to me, was to display the correct local time at the required location.

### Future Development:

Currently the API key is hardcoded within the JS file. As such, anyone can view the key simply using their browser's developer tool. Storing API keys directly in client-side scripts, in this way, is a major security vulnerability. To remedy this, a solution was scoped to build a proxy server to deal with API authentication in server-side script. A solution was built and tested, employing a node.js environment. However, it was decided that this solution was beyond the scope of this project. So, the solution was shelved, to be revisited in a later module.

---

## GitHub

### GitHub repository:

My solution is contained within a project called: W5-Challenge-Mayer.  
The project has now been pushed my GitHub repository: https://github.com/paulmayer-fullstacker/week-5/


### GitHub Pages:

The solution has been published to GitHub Pages, and can be found at this URL:  
https://paulmayer-fullstacker.github.io/week-5/W5-Challenge-Mayer/

---

## To Conclude:

I hope that that this submission is adequate and appropriate, at this stage of the course.

---

<br/>

<hr style="height: 5px; background-color: black; border: none;">
