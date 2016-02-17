P4: Website Optimization Course Readme

######################################################
#ABOUT
######################################################
Created by Chris Blackden for Udacity P4
2-16-16
Readme 1.0

######################################################
#HOW TO RUN
######################################################
Assumptions:
You have installed a web server and ngrok on your machine
(I used SimpleHTTPServer, but IIS will work for Windows clients if you can configure it)

SimpleHTTPServer Tutorial
http://www.pythonforbeginners.com/modules-in-python/how-to-use-simplehttpserver/

Ngrok Homepage
https://ngrok.com/

IIS Setup Documentation
http://windows.microsoft.com/en-us/windows7/install-internet-information-services-iis-7-5

From Terminal:
cd <Put project folder here>
python -m SimpleHTTPServer 8080 (If you are using a different web server, substitute that for this step)
Open a 2nd terminal window
cd <Put project folder here>
ngrok 8080
Open the URL that is displayed in the 2nd terminal window in a browser. It should be something similar to http://XXXXXXXX.ngrok.com
Enter that URL for PageSpeed Insights at https://developers.google.com/speed/pagespeed/insights/

######################################################
#CHANGES MADE
#There may be some missing I did not start this readme file until after turning in the project
######################################################
1. Minified CSS for Google Fonts API in Index.html and inlined it at the top of the page
2. Moved CSS calls to bottom of index.html for faster loading
3. Reduced number of pizzas in background in line 541 of main.js
4. Moved variable creation outside of loop in main.js at lines 483 and 464
5. Commented out DetermineDX function in main.js from line 419 to 447 as it was only used once and was unnecessary 
6. Simplified ChangePizzaSizes function in main.js from line 449 to 471
7. Converted pizzaria.jpg into pizzaria.png on line 40 of pizza.html and line 62 of index.html