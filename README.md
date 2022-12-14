# Web Design Challenge
## Glen Dagger
### Module 11 Challenge

---

For this assignment, I used HTML, CSS, and CSS Bootstrap to create a dashboard featuring the Latitude vs. X analysis of weather. This project used the provided data set and images from the WeatherPy assignment as the primary source of content.

<br>

---

<br>

### Landing Page

The landing page is coded in the 'index.html' file in the main repository folder. This page provides an overview of the project, an example of one of the plots, and a "Visualizations" sidebar containing four images of the plots as links to their own visualization page (Temperature, Humidity, Cloudiness, and Wind Speed).

<br>

---

<br>

### Visualizations

Each visualization page contains a header, a regular-sized scatter plot image for the selected comparison, and a brief paragraph describing the plot. All visualization images are stored in the "assets/images" folder in the main repository. Each page also contains the same visualization sidebar section as the landing page with links to their respective pages.


<br>

---

<br>

### Navigation Bar

Every page contains a navigation bar that was created as a Bootstrap component and customized to roughly match the color/layout/general appearance of the screenshots. It contains the name of the site on the lefthand side that links to the landing page, links to the "Data" and "Comparisons" page, and a working dropdown with links to each of the four visualization plot pages. This navbar collapses when the window is reduced in size and changes color on small screens (using a media query).


<br>

---

<br>

### Data Page

The "Data" page contains a table of the original CSV file used to generate the visualizations and analysis. This was created in the 'data_table.ipynb' Jupyter notebook file in which I used Pandas to read in the csv file and export it as an HTML file. I then used an HTML Include function to embed this table into the "Data" page, and used CSS to format the table to be striped and to highlight rows hovered over by the user's mouse.

<br>

---

<br>

### Comparison Page

The "Comparison" page contains all four images for a visual comparison with correct labels. Using CSS Bootstrap, and columns are responsive so that they are laid out 2x2 on large screens and 4x1 on small screens.  All images link to their respective visualization page. CSS was used to add a border to each image here (as well as to images in the Visualization sidebar on the other pages) when the user hovers over it with the mouse. Media queries were included to separate images with a horizontal rule only on screen sizes 991px and smaller, and are otherwise hidden.

<br>

---

<br>

### Folder Organization

The Landing page (index.html), Comparison page (comparison.html), and Data page (date.html) are stored in the main repository folder. This parent directory also contains the following:
  
- Visualizations folder
  - Visualization pages
    - cloudiness.html
    - humidity.html
    - temp.html
    - wind.html
  
- Assets folder
  - CSS folder
    - CSS style sheet
  - Images folder
    - four visualization plot images
