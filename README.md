# Website-Optimization
Udacity Front-End Web Developer Nanodegree Project-4

## About
The main goal for this project is was to optimize [Cameron Pittman's portfolio](https://github.com/udacity/frontend-nanodegree-mobile-portfolio) page for speed so that it achieves a PageSpeed score
of 90 (on index.html) and runs at 60 frames per second (when scrolling in pizza.html) on both mobile and desktop environments,
using techniques  you've picked up in [The Critical Rendering Path course](https://www.udacity.com/course/website-performance-optimization--ud884).

## How to run
To run the site, you have to download  all files of this repo, and to open the index.html in a browser locally 
or to click [here](http://webbdev.github.io/Website-Optimization/).

Changes made to optimize the site:
## Part 1: Optimize PageSpeed Insights score for index.html

1. Set async attribute to synchronously load low priority scripts in analytics.js, perfmatters.js  and moved to the end of the closing body tag </body>;
2. Set media query for print stylesheet (css/print.css);
3. For Google fonts, removed the 700 size fonts (the bold font) as it was not used and minimized the number of critical resources (JavaScript and CSS) by combining and compressing multiple files in order to reduce load time, as well as the number of http requests.
4. Minified CSS files.
5. Made validate HTML, CSS, JavaScript codes, using online Validators.
6. Optimized images: images were resized and compressed.
7. Added .htaccess file in the root of the website.
This file contains the necessary configurations to help improve the web site's performance and security.
1) Expires and Cache-Control headers for images, static files, CSS, JavaScript, media files, web fonts, and others. This helps in serving the page faster because it avoids unnecessary HTTP requests when the user reloads the page the second time.
2) Gzip compression Enabled for serving compressed HTML, CSS scripts, and any other type of text content.

## Part 2: Optimize Frames per Second in pizza.html

1. Made validate HTML, CSS, JavaScript codes, using online Validators.
2. Optimized JavaScript  in views/js/main.js.
   Made loop optimization.
3. Made measuring with Navigation Timing.

_Before optimization:_

![alt tag](https://raw.githubusercontent.com/webbdev/Website-Optimization/master/img-timeline/pizza-measure-before.png)


_After optimization:_

![alt tag](https://raw.githubusercontent.com/webbdev/Website-Optimization/master/img-timeline/pizza-measure-after.png)

### Tools used in the optimization process:

   * [Google Chrome Developer Tools](https://developer.chrome.com/devtools) - to measure performance.   
   * [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) - to measure pages speed.
   * Paint , Image Compressor - to reduce images sizes while keeping the highest quality possible.
   * HTML, CSS, JavaScript Compressor - to reduce files sizes.
