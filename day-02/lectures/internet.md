##SWABTS:
***Explain how loading a web page in your browser works***

## Motivation / Why Should You Care?
How many times a day do you use the internet? How many times do you load a different web page? I bet you can't even begin to guess how many times in a year! In order to be a developer, and especially a web developer, it's incredibly important to understand how the web works.

## Lesson Plan
+ Been previewing the sites you’ve been working on by using your browser to open up the local files on your computer.
+ When visit www.flatironschool.com your browser is making a request from your computer to a remote server where the files for the Flatiron School website are hosted. 
  * A server is a just a big computer that runs the code for that website
+ Websites and computers have their own addresses just like apartments do, it's how messages get sent back and forth
+ IP addresses are random sequences of letters and numbers 
  * it's hard to remember so we just use URLs for websites that point to an IP address
  * We can see the IP address for flatironschool.com by going to our terminal and entering `ping flatironschool.com`
  * Google `what’s my IP address` to find your computer's
+ When you go to `www.flatironschool.com` you are making an HTTP request- a GET request to Flatiron School's server. Your IP address gets sent along with your request so the server knows where to send back the info
  * flatironschool.com sends back your IP address all the html and css files to create the page
+ We’re going to use Github as the server to host your website. This means we need to set up a new repository for your site on Github and push up files from your local computer up to Github so people anywhere in the world can access them and visit your site.


## Conclusion / So What?
Both computers and websites have their own unique IP addresses, which allow open communication for requesting and recveing information on the internet.

## Hints and Hurdles
+ IP addresses and HTTP requests is like texting!