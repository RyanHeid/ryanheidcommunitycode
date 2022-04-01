# Community Code Project

## About My Community

I picked the DEV community to engage with their JavaScript community. I've been happy with my choice, as it has proven to be a place where I have been able to find useful information about topics I am interested in JavaScript, as well as other programming languages like Kotlin or Python. I have built a website for my podcast, called Inside the Minds Podcast. One of my intentions of joining the DEV community was to search their resorces to find ways that I could imporve my website's HTML, CSS and JavaScript coding. Through trial and error, I was able to find some JavaScript code that I could implement on my website. I also found some code that I was not able to implement on my site. Not because it was bad code, or faulty code, but more so because of how I coded my website. 

## Light/dark mode toggle switch
After searching through some ideas, I found some code that allowed me to switch between a light and dark mode in the body of my website. This change works on a toggle switch that is below my navigation, near the top left of the screen. The "light" color is orange, and the "dark" color is a shade of black. I chose these colors because these are the colors of my website. I like how this turned out, although I am not sure that I will keep it. <br>
Here is the HTML for the toggle switch: <br>
``` html
<div> 
    <input type="checkbox"
    class="checkbox" id="checkbox">
    <label for="checkbox"
    class="label">
    <span class="ball"></span>
    </label>
</div>
```
<br>
Here is the JavaScript for the toggle switch: <br>
HTML:<br> 
<br>
``const checkbox =`` <br>
``document.getElementById('checkbox');`` <br>
``checkbox.addEventListener('change', () => {`` <br>
``doucument.body.classList.toggle('dark');`` <br>
``});`` <br>
<br>
The code I referenced from was posted by Abbey Perini Nov 06, 2021 https://dev.to/abbeyperini/an-accessible-dark-mode-toggle-in-react-aop <br>
<br>
HTML: <br>
```html
<div className="container--toggle">
    {
        togClass === "light" ?
            <input type="checkbox" id="toggle" className="toggle--checkbox" onClick={handleOnClick} checked />
        :
            <input type="checkbox" id="toggle" className="toggle--checkbox" onClick={handleOnClick} />
     }
     <label htmlFor="toggle" className="toggle--label">
          <span className="toggle--label-background"></span>
     </label>
</div>}
```
JavaScript:
```javascript
const handleKeypress = e => {
  if (e.key === "Enter") {
    if (localStorage.getItem('theme') === 'theme-dark') {
      setTheme('theme-light');
      setTogClass('light')
    } else {
      setTheme('theme-dark');
      setTogClass('dark')
    }
  }```

## Radio Button Confirmation
I searched my community looking for a way to interact with a radio button in my form. I found a code snippet that displays if a radio button is checked, or unchecked.  Although I did not find exactly what I was looking for at the time, I made some modification to the code and changed it into code that would show the user what radio button they clicked after pressing a button. Here is my code. <br>
HTML: <br>
```html
   <form id="form-user" method="post" onsubmit="return checkForm(this);" action="https://learndigital.dev/programs/dgl103-form.php">
            <label for="fname">First Name</label><br>
            <input type="text" id="fname" name="firstname" placeholder="Ex: Mike">
            <br>
        <label for="lname">Last Name</label><br>
        <input type="text" id="lname" name="lastname" placeholder="Ex: Smith">
            <br>
        <label for="email">Email </label><br>
        <input type="text" id="email" name="email" placeholder="Ex: ryan@gmail.com" required>
        <input type="submit" value="Submit">
        <br>
 ```
 
 JavaScript: <br>
 ```javascript
 function myFunction() {
  let date = document.forms[0];
  let txt = "";
  let i;

  for (i=0; i < date.length; i++){
if (date[i].checked) {
 txt = txt + date[i].value + "";
}
document.getElementById("results").value = "Selected date is: " + txt;
  }
```
The code I referenced from was posted by Codeanddeploy on Mar. 23 https://dev.to/codeanddeploy/how-to-unchecked-a-radio-button-using-javascriptjquery-1h1f <br>
HTML: <br>
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>How to unchecked a radio button using JavaScript/jQuery?</title>
</head>
<body>
    <h1>How to unchecked a radio button using JavaScript/jQuery?</h1>

    <form id="form1">


        <p><b>Current Status</b></p>
        <input type="radio" value="1" name="status" class="status" checked> Active

        <br/><br/>

        <button type="button" id="btnSubmit">Deactivate</button>
    </form>
</body>
</html>
```
<br>
JavaScript:
```javascript
 <script type="text/javascript">
        $(document).ready(function() {
            $("#btnSubmit").on("click", function() {
                var status = $(".status");
                status.prop("checked", false);
            });
        });
    </script>
```    

        


