# project-website-template .
Demo: https://yenchiah.github.io/project-website-template/

This is a responsive (mobile/desktop) and light-weight HTML/CSS template for building projects or personal websites. If your website does not require complex user interactions, I recommend starting with the empty template (empty.html) and copy codes from the file that contains different layouts (index.html). For building interactive websites, this library also provides several widgets (widgets.html) based on [jQuery](https://jquery.com/) and [jQuery UI](https://jqueryui.com/). Two examples that use this template are:
- Project webstie: [http://smellpgh.org](http://smellpgh.org)
- Personal website: [http://yenchiah.me](http://yenchiah.me) .

If you would love to keep updating this template, please keep your codes in separate files (custom.css and custom.js) and avoid modifying the followings:
- css/frame.css (CSS for the main frame of the website)
- css/controls.css (CSS for control elements that do not require JavaScript)
- css/widgets.css (CSS for widgets that require JavaScript)
- js/widgets.js (JavaScript for widgets)
- js/menu.js (JavaScript for loading the menu bar)

From version 3.0, the menu bar at the top is moved into a single file (menu.html) for better management. Each template page will now use jQuery to load the menu bar file (menu.js), as shown below:
```html
<script src="js/menu.js"></script>
```
If your website is static and requires no user interactions, I recommend copying the code from the menu file (menu.html) into the menu-container div in your html template.
```html
<div class="menu-container">
  [copy everything in the menu.html and paste the code here]
</div>
```
In this way, you can remove the script line that loads jQuery in the header of the html and also delete the files for loading the menu bar (menu.html and menu.js).

This template is tested and worked on:
- MAC Desktop Chrome 71.0.3578.98
- Android Mobile Chrome 71.0.3578.98
- MAC Desktop Firefox 64.0
- Android Mobile Firefox 64.0
- MAC Desktop Safari 12
- iOS Mobile Safari 12

# Known Problems and Bugs

Here are several known problems and bugs that will be addressed in a later version:

- The dropdown menu in the widget has clicking problems on Windows Firefox.
- On mobile Safari, the menu on the top will not close after opening it. This is because the menu icon on mobile Safari retains focus after a touch event, and the menu relies on the loss of focus event of the icon to close.


# Future Plans

Here are several planned features that will be add in the future:

- A slideshow block for showing images or videos
- A footer at the bott
