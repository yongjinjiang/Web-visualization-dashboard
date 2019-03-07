## About
   - This is the personal project for unit 12(Web) of [Data Visualization and Analytics](https://bootcamp.umn.edu/data/landing%20full/)(graded A).
   - Bulit a dashboard to visualize the lattitude dependence of the global weather. The dataset and figs are fed from another project(i.e., [homework project](https://github.com/yongjinjiang/Python-API) for unit 06(Python-APIs)), in which  the weather for more than 500  randomly chosen cities were collected from the [openweathermap API](https://openweathermap.org/api) for current  date. For more details, see [here](#the-original-text-of-the-homework-assignment).
   - A snapshot of the app: 
<img src="./Images/app.png " width="600" height="400">

   - The web-link for the app of this project is [here](https://yongjinjiang.github.io/Web-visualization-dashboard/).
   - Main tools used in this project: html, css, [Bootstrap](https://getbootstrap.com/).
   
## Usage 
   - Clone this repo as well as the [repo for Python-APIs](https://github.com/yongjinjiang/Python-API). Use the main.ipynb of the second repo to generate a new list of cities and collect new png figures for the current weather data. Feed those figures into ./Resources folder of the current project. Then, you can open the index.html and play with the dashboard. You might get different observations from mine described in the following. 
   
## Some observations
   - From the weather data for 538 cities collectd today(11/07/2018), we conclude that temperature is peaked around 80 Fahrenheit near the equator from -20 to 30 degrees of Latitude. It continually drops to 30 Fahrenheit(even lower for several cities) in the region of 40 to 80 degree of latitude.
   - There is no obvious dependence of cloudiness on latitude. Yet somehow there are several cloudiness values, 0, 20, 40, 78,97, are most crowded with citis all over the world, much more than other values.
   - The humidity percentage has only weak dependence on the latitude. It takes smallest value around -20(Southern Hemisphere) and 20 latitude(Northern Hemisphere).
   - There is no obvious dependence of wind speed on latitude. The wind speed in general is from 0 mph to 15 mph.

## **_The original text of the homework assignment:_** 
# Unit 12 | Assignment - Web Visualization Dashboard (Latitude)

## Background

Data is more powerful when we share it with others! Let's take what we've learned about HTML and CSS to create a dashboard showing off the analysis we've done.

![Images/landingResize.png](Images/landingResize.png)

## Latitude - Latitude Analysis Dashboard with Attitude

For this homework we'll be creating a visualization dashboard website using visualizations we've created in a past assignment. Specifically, we'll be plotting [weather data](Resources/cities.csv).

In building this dashboard, we'll create individual pages for each plot and a means by which we can navigate between them. These pages will contain the visualizations and their corresponding explanations. We'll also have a landing page, a page where we can see a comparison of all of the plots, and another page where we can view the data used to build them.

### Website Requirements

For reference, see the ["Screenshots" section](#screenshots) below.

The website must consist of 7 pages total, including:

* A [landing page](#landing-page) containing:
  * An explanation of the project.
  * Links to each visualizations page.
* Four [visualization pages](#visualization-pages), each with:
  * A descriptive title and heading tag.
  * The plot/visualization itself for the selected comparison.
  * A paragraph describing the plot and its significance.
* A ["Comparisons" page](#comparisons-page) that:
  * Contains all of the visualizations on the same page so we can easily visually compare them.
  * Uses a bootstrap grid for the visualizations.
    * The grid must be two visualizations across on screens medium and larger, and 1 across on extra-small and small screens.
* A ["Data" page](#data-page) that:
  * Displays a responsive table containing the data used in the visualizations.
    * The table must be a bootstrap table component.
    * The data must come from exporting the `.csv` file as HTML, or converting it to HTML. You may use a csv-to-html table conversion tool, e.g. [ConvertCSV](http://www.convertcsv.com/csv-to-html.htm).

The website must, at the top of every page, have a navigation menu that:

* Has the name of the site on the left of the nav which allows users to return to the landing page from any page.
* Contains a dropdown on the right of the navbar named "Plots" which provides links to each individual visualization page.
* Provides two more links on the right: "Comparisons" which links to the comparisons page, and "Data" which links to the data page.
* Is responsive (using media queries). The nav must have similar behavior as the screenshots ["Navigation Menu" section](#navigation-menu) (notice the background color change).

Finally, the website must be deployed to GitHub pages.

When finished, submit to BootcampSpot the links to 1) the deployed app and 2) the GitHub repository.

### Considerations

* You may use the [weather data](Resources/cities.csv) or choose another dataset. Alternatively, you may use the included [cities dataset](Resources/cities.csv) and pull the images from the [assets folder](Resources/assets).
* You must use bootstrap. This includes using the bootstrap `navbar` component for the header on every page, the bootstrap table component for the data page, and the bootstrap grid for responsiveness on the comparison page.
* You must deploy your website to GitHub pages, with the website working on a live, publicly accessible URL as a result.
* Be sure to use a CSS media query for the navigation menu.
* Be sure your website works at all window widths/sizes.
* Feel free to take some liberty in the visual aspects, but keep the core functionality the same.

### Bonuses

* Use a different dataset! The requirements above still hold, but make it your own.
* Use a bootstrap theme to customize your website. You may use a tool like [Bootswatch](https://bootswatch.com/). Make it look snazzy, give it some attitude. If using this, be sure you also meet all of the requirements listed above.
* Add extra visualizations! The more comparisons the better, right?
* Use meaningful glyphicons next to links in the header.
* Have visualization navigation on every visualizations page with an active state. See the screenshots below.

### Screenshots

This section contains screenshots of each page that must be built, at varying screen widths. These are a guide; you can meet the requirements without having the pages look exactly like the below images.

#### Landing page

Large screen:
![Landing page large screen](Images/landing-lg.png)

Small screen:
![Landing page small screen](Images/landing-sm.png)
￼

#### Comparisons page

Large screen:
![comparison page large screen](Images/comparison-lg.png)

Small screen:
![comparison page small screen](Images/comparison-sm.png)

#### Data page

Large screen:
![data page large screen](Images/data-lg.png)

Small screen:
![data page small screen](Images/data-sm.png)

#### Visualization pages

You'll build four of these, one for each visualization. Here's an example of one:

Large screen:
![visualize page large screen](Images/visualize-lg.png)

Small screen:
![visualize page small screen](Images/visualize-sm.png)

#### Navigation menu

Large screen:
![nav menu large screen](Images/nav-lg.png)

Small screen:
![nav menu small screen](Images/nav-sm.png)
