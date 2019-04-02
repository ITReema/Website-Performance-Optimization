## Website Performance Optimization


### Instructions Running:
There are two ways for you to run the application:

* Clone the GitHub repository at:
```
  git clone https://github.com/ITReema/WebsitePerformanceOptimizationportfolio.git
```

* if you want Open the application in localhost: 
1. Download the repository and open index.html in your own browser.
2. Download and install [ngrock](https://ngrok.com) and put ngrok file in project folder.
3. Open Terminal to run a local server 
  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```
4. Open a browser and visit localhost:8080
5. Open new window Terminal to make your local server accessible remotely
  ``` bash
  $> cd /path/to/your-project-folder
  $> ./ngrok http 8080
  ```
6. Copy the public URL ngrok gives you and try running it.


#### Part 1: Optimize PageSpeed Insights score for index.html

1. Remove Google font.
2. Minified and inlined style.css.
3. Added async attribute to links (stylesheet and script).
4. add media="print" to link print.min.css.

#### Result PageSpeed Insights: 

the webpage received a speed score of 99/100 for Mobile and 95/100 for desktop.
[Result](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Frawgit.com%2FITReema%2FWebsitePerformanceOptimizationportfolio%2Fmaster%2Findex.html&tab=desktop)

#### Part 2: Optimize Frames per Second in pizza.html

1. add viewport tags to pizza.html.
2. Minified style.css.
3. function changePizzaSizes Reduce time resize pizzas from ~200 ms to < 5 ms.
4. function updatePositions add global varibal and chnge querySelectorAll to getElementsByClassName.
5. creates the moving pizzas in rows and cols layout. 
