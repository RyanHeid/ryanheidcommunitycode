# Community Code Project

## About My Community

I picked the DEV community to engage with their JavaScript community. I've been happy with my choice, as it has proven to be a place where I have been able to find useful information about topics I am interested in JavaScript, as well as other programming languages like Kotlin or Python. I have built a website for my podcast, called Inside the Minds Podcast. One of my intentions of joining the DEV community was to search their resorces to find ways that I could imporve my website's HTML, CSS and JavaScript coding. Through trial and error, I was able to find some JavaScript code that I could implement on my website. I also found some code that I was not able to implement on my site. Not because it was bad code, or faulty code, but more so because of how I coded my website. 

## Light/dark mode toggle switch
After searching through some ideas, I found some code that allowed me to switch between a light and dark mode in the body of my website. This change works on a toggle switch that is below my navigation, near the top left of the screen. The "light" color is orange, and the "dark" color is a shade of black. I chose these colors because these are the colors of my website. I like how this turned out, although I am not sure that I will keep it. <br>
Here is the HTML for the toggle switch: <br>
<br>
``<div>`` <br>
``<input type="checkbox">`` <br>
``class="checkbox" id="checkbox">`` <br>
``<label for="checkbox"`` <br>
``class="label">`` <br>
``<span class="ball"></span>`` <br>
``</label>`` <br>
``</div>`` <br>
<br>
Here is the JavaScript for the toggle switch: <br>
<br>
``const checkbox =`` <br>
``document.getElementById('checkbox');`` <br>
``checkbox.addEventListener('change', () => {`` <br>
``doucument.body.classList.toggle('dark');`` <br>
``});`` <br>
<br>
The code I refrenced from was posted by Abbey Perini Nov 06, 2021 https://dev.to/abbeyperini/an-accessible-dark-mode-toggle-in-react-aop <br>
<br>
``<div className="container--toggle">`` <br>
``    {`` <br>
``        togClass === "light" ?``<br> 
``            <input type="checkbox" id="toggle" className="toggle--checkbox" onClick={handleOnClick} checked />`` <br>
``        :`` <br>
``            <input type="checkbox" id="toggle" className="toggle--checkbox" onClick={handleOnClick} />`` <br>
``     }`` <br>
``     <label htmlFor="toggle" className="toggle--label">`` <br>
``          <span className="toggle--label-background"></span> ``<br>
``     </label>`` <br>
``</div>`` <br>
<br>

