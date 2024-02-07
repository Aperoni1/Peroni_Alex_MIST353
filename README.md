# Alex Peroni
## Assignment 2
### 1/26/2024

**Similar Websites:**

1. [Forest Service Fire Information Website](https://www.fs.usda.gov/science-technology/fire/information#:~:text=InciWeb%20is%20an%20interagency%20all,%2C%20hurricanes%2C%20tornadoes%2C%20etc.)
   - This is the Forest Service’s fire information website. The website features an interactive map that is in a frame and is linked to [Wildfire Map](https://maps.wildfire.gov/sa/#/%3F/%3F/30.2164/-108.6803/5). The map allows for the collection of user location data, but that feature does not work on the website. The map features icons that can be clicked on. When clicked on, a pop-up opens and more information about the icon is displayed. The icons are divided into layers that make up sections of the map. Additionally, the icons are images that are 10x10 pixels. I like the features that are on this map, and I would like to integrate a similar feature to my application if possible.

2. [National Weather Service Weather and Hazards Map](https://www.weather.gov/fire/)
   - This is the National Weather Service’s weather and hazards interactive map. This site allows users to interact with a map that, like the previous site, is linked to another webpage that features the interactive map. ([Interactive Map](https://www.wrh.noaa.gov/map/?&zoom=4&scroll_zoom=true&center=38.47939467327645,-98.701171875&basemap=ESRI%20Topographic&sidebar=hide&boundaries=false,false,false&hazard=true&hazard_type=fire&hazard_opacity=60)) This site is slightly different because it features weather data and hazard data. This map uses colored areas to indicate hazards. These areas appear to be controlled by JavaScript, since I can’t find any HTML that appears to be linked to them. Additionally, the interactive map can be replaced with images of forecast maps that fit into the same frame. Overall, I like this design better than the previous site, but it may be more challenging to implement a design similar to this because of the JavaScript involved.

3. [West Virginia Division of Forestry Wildfire Danger Map](https://wvforestry.com/wildfire-danger-map/)
   - This is the West Virginia Division of Forestry’s wildfire danger map. This website is incredibly basic. Instead of an interactive map, the website features a button that links to a .PNG that is updated daily by the Division of Forestry. The webpage uses JavaScript to link to the various other sections of the website. I do like the simplicity of the website, but I would like to implement more features on my pages. I do really like the way the other pages are linked. They have buttons with images that have a slight shade on them when you hover the mouse over them.

**GitHub Repositories:**

1. [jVectorMap](https://github.com/bjornd/jvectormap)
   - This repository contains JavaScript for the jVectorMap. This is an interactive map that allows for customizable markers and labels. Additionally, it allows for full zooming and panning. It features maps of all countries and continents. This library is highly developed and has its own dedicated website with pricing tiers for commercial and personal use. The creators allow for free personal use if all source code and modifications to it are publicly available. I would like to try to integrate this into my design if possible.

2. [Simple React Weather App](https://github.com/konstantinmuenster/simple-react-js-weather-app?tab=readme-ov-file)
   - This repository is a simple weather application that uses the open weather API. ([Open Weather API](https://openweathermap.org/api)) It gets the weather for the city that the user enters. I would like to integrate a similar feature to my page that allows the user to use their location or a city that they enter. If I integrate a feature like this, I would like to have a forecast and maybe a fire risk indicator that uses the location that the user inputs.

**Future work:**
- I tried to implement the interactive map, but I was unable to display it. I will need to do more research on jVectorMap to properly implement it. Additionally, I did not attempt to implement the weather feature. Going forward, I will implement it along with the user location feature.

**AI Use:**
- I used ChatGPT 3.5 to generate the button on my about page that toggles the table. 
    - I entered the prompt: make a js button that hides and unhides ftrTbl: 
    ```html
    <div class="container">
        <table class="ftrTbl table">
            <thead>
                <tr>
                    <th>Potential Features</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Interactive Map</td>
                </tr>
                <tr>
                    <td>User location data</td>
                </tr>
                <tr>
                    <td>Weather data for the users location</td>
                </tr>
            </tbody>
        </table>
    </div>
    ```
    - ChatGPT Response: ChatGPT gave me this JavaScript implemented into my existing code. It works well, but I had to modify my CSS to change the button color to green.
    ```html
    <button id="toggleBtn" class="btn btn-primary">View Features</button>

    <!-- JavaScript to toggle visibility of the table -->
    <script>
        document.getElementById('toggleBtn').addEventListener('click', function () {
            var table = document.getElementById('ftrTbl');
            if (table.style.display === 'none') {
                table.style.display = 'table';
            } else {
                table.style.display = 'none';
            }
        });
    </script>
    ```

