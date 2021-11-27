### I've updated everything, a quick run down to explain it:
 
> ```index.md``` markdown file that holds the main content of the site. This is the file we edit to add stuff to the site.

> ```_config.yml``` contains the options for the site. (Used by jekyll to fill in banner, footer and set theme).

> ```_layouts/default.html``` The current template is identical to default but by having it here we can customise the html if needs be. 

> ```assets/``` 
> - ```css/style.scss``` allows us to customise css if needs be.
> - ```Logo.png``` logo isnt used in this template, can modify ```default.html``` to add logo if we need it.

> ```README.md``` this file.

### To change the theme:
1. update ```remote_theme: pages-themes/cayman@v0.2.0``` in ```_config.yml```
2. replace ```/_layouts/default.html``` with default template taken from theme repo. Can find the compatible themes [here](https://github.com/pages-themes).
   Cayman default theme can be found [here](https://github.com/pages-themes/cayman/blob/master/_layouts/default.html).
3. I think all themes linked above use ```site.theme``` so shouldnt be an issue but if first two steps dont work, try commenting out the import statement in ```/assets/css/style.scss```.

Again, this is the default Cayman teplate. We can alter the ```default.html``` to modify it or feel free to change the theme to a new one. Just wanted to get the folder structure somewhat set up.
