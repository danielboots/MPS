# **Milestone Project 1**  - User Centric Frontend Development.

## **Music Production Service** - _Music Consultancy and Service Business_

![MPS logo and strap line ](/images/mpslogostrap.png)


---
## **About the project:**

**Music Production Service** is my own business which i run successfully in the music industry. 
I decided to approach rebuilding the website using the skills i have learned so far from the first modules of the **'Full Stack Developer Course'** from **Code Institute**.

I aim to complete the website following web best practices and also to fulfill my need to present my business information on a website which is not only well structured but is also mobile responsive. 

It should have a a professional look about it and also is not overly complicated with regards to UX navigation and content layout so that potential clients can visit the website and find what they are looking for.


As a business owner my end goal is to convert visitors to the site to customers not only that but to capture leads through contact forms and relevant _call to actions_ such as **newsletter signup forms**.


## **Technologies Used:**
___

* **[HTML](https://developer.mozilla.org/en-US/docs/Web/HTML):** - Is the main language used in this project which allowed me to correctly structure the website, whereby using best practices to use semantic tags where appropriate.

* **[CSS](https://developer.mozilla.org/en-US/docs/Web/CSS):** - Was used via an external stylesheet using best practices to style format and visually present the HTML.

* **[JAVASCRIPT](https://developer.mozilla.org/en-US/docs/Web/JavaScript):** - *As part of Bootstrap* Javascript although i havent programmed it, was included in the site as part of the Bootstrap framework so that some Bootstrap components such as the navigation toggler would work.

* **[JQUERY](https://jquery.com/):** - *Again only employed as part of Bootstrap so that Bootstrap components work as expected.*

* **[BOOTSTRAP](https://getbootstrap.com/):** - The framework for the site allowing use of the Bootstrap grid and responsive mobile first approach. I Used many components from Bootstrap mainly, the Carousel, Nav bar, forms and modals. 

* **[GITPOD](https://gitpod.io/):** - IDE for this project. Allowed me to fork the Code Institute template from Github and open in Gitpod so that all extenstions were available.

* **[GIT](https://git-scm.com/):** Git employed as version control

* **[GITHUB](https://github.com/):** - Github was used to host the repository for this project.

* **[SQUOOSH](https://squoosh.app/):** - I used Squoosh in order to reduce the image sizes

* **[PHOTOSHOP](https://www.adobe.com/uk/products/photoshop.html):** - For editing images associated with this project.

* **[BALSAMIQ](https://balsamiq.com/):** - Mac version to develop wireframes for this project.

___



## **UX:**
___
I have carried out a full UXD report as this is a functioning business already operating and 
UX has never been addressed it would be a good time as ever to carry one out. The full report can be found here: **[UXD Report](/assets/UXD-MPS.pdf):**

For your reference i have also provided a general overiew of my analysis. 


### **Strategy plane: The Initial idea.**
___
The strategy plane or initial idea for this project centres around coupling a rebuild of a current website using the latest technologies I have learned to also satisfy my user centric front end design milestone project. 
Primarily I am aiming to tie in real life applications and not 'concepts' with all of my projects so that I have to address all issues and strategy from a real world stand point.


## **Features:**
___



## **Testing:**
___

Testing was an integral part of the design and build process, responsiveness is cruicial to the success of any online website so a number of steps were employed to ensure that the site worked across a number of platforms and browsers.
Not only responsiveness but positioning, colours, inheritence etc were all factors to be taken into consideration, thus Google Chrome developer tools was used extensively to test all aspects of the site.
Although Bootstrap is a mobile first approach i opted to work on a simple desktop version first as i could work backwards.
I first of all set up a few .css rules for the body section which allowed me to set some global rules such as.

<!-- Code Blocks -->
``` Css
  * {
  box-sizing: border-box;
}
```
Which made sure that i was working with the box model more logically. 

##Real world example of debugging using Chrome Dev tools.

Chrome dev tools also allowed me to test inheritence in _**CSS**_ and test different rules and sizing to ensure that my content was displaying correctly on a number of browsers and screen size emulations.
One such example was when i was nearing the end of the project where i found that the Hero text **Music Production Service** displayed in the center on all screen resolutions but not on my Apple iPhone it was pushed further down than expected. 

Screenshot 1 : Opening the website in dev tools.

![Screen1-Devtools-testing](/images/devtool1.png)

Screenshot 2 : Ammending the .css rule and making a media query to fix

![Screen2-Devtools-css-fix](/images/devtool2.png)


I opened the dev tools inside of Chrome and adjusted the screen size and made the correct media query to remedy the issue using this media query. 


``` Css

@media all and (max-width: 425px) {
    .hero-text {
    text-align: center;
    position: absolute;
    top: 30%;
    left: 10%;
    right: 10%;
    color: white;
}
```

One other major factor i came across is when using `.container-fluid` my content was as expected at full width across the screen, which for some sections i liked but on bigger screen resolutions i found for UX purposes i needed to set a max width so that the content didnt spread across the page. I found this looked sloppy and not good in terms of design. I tested this too out with dev tools to create a `.container-max` rule which for large screen resolutions the content was displayed better.


## **User Experience testing:**

As this website is aimed at getting clients to interact with the site through booking or enquiring about a service i had to ensure that in my testing i adequately tested the UX and that it was simple enough for the user to "learn" how to use the site and follow industry standards and user expectations. 

* This translated in to me using a top menu bar with LOGO positioned to the left and menu items positioned on the right. 
* Mobile responsiveness i chose to have a right hand side positioned Hamburger / toggler nav which presented the menu options in a neat and decluttered way. 
* I used many inbound links and tested all links ensuring that they all work and link correctly.
* All social media icons link to the right external pages using the `target="_blank"` attribute so that external pages are opened in a new tab.
* I tested all parts of the website including Bootstrap components, as i used:  
    1. the NAV bar - Tested on all pages and on Firefox, Chrome and Safari, also on iOS iPhone all working correctly. 
    1. Modal as a button CTA which includes an enquiry form - Although the form isnt functioning it was tested again Tested on all pages and on Firefox, Chrome and Safari, also on iOS iPhone all working correctly.
    1. Carousel for testimonials - Tested on all pages and on Firefox, Chrome and Safari, also on iOS iPhone all working correctly.




### **Utilising Mentor Sessions:**
After my initial mentor session to discuss the idea and scope of the project i made sure that i could bring the project as far to completion as possible so that i could use his expertise in our next session. 
I had a number of issues which Allen helped me rectify. Notibly the Navbar brand logo sizing, a carousel issue and footer links which have been noted as comments in my .CSS file.

### **Further Testing:**

* The use of validation services for **[Jigsaw CSS Validator](https://jigsaw.w3.org/css-validator/)** and **[HTML Validator](https://validator.w3.org/)** allowed me to modify and fix any errors in my code, one highlight of using these validation services especially in CSS was that i was repeating alot of the same rules for font colour, the validation service allowed me to remove alot of  those rules and condense them into one rule which made a lot more sense.

* I finally used **[GTMETRIX](https://gtmetrix.com/)** which is used to test page website speeds. All testing came back fine apart from image sizes which scored pretty low. Thus i used the free online **[SQUOOSH](https://squoosh.app/)** to reduce massive image sizes upto 80% of their original file size. This is especially important as large image sizes dramatically increase page loading speeds and leads to a bad UX especially on mobile where heavy loading sites can eat data very quickly. 

### **Testing Issues:**

One issue which doesnt affect UX but didnt pass the validation was the inclusion of youtube embed code, specifically the **iframe** i will add this to my future development so that i can embed youtube videos without the need of **iframe**

### **_HTML Validation error when using Youtube embed._**
![iframe testing error on HTML validator](/images/Iframe.png)


___




## **Deployment:**
This project was developed using the Gitpod IDE which integrates seemlessly with Github, Git pod is a cloud IDE so this allowed me to work at home on my imac or out on my imac using only an internet connection and the website **[GITPOD workspaces](https://gitpod.io/workspaces/).** 

The site was developed inside of the Gitpod IDE and connected to my GitHub repository. 
As sections of the site were completed i ensured that i used version control to maintain copies of my code on the repository. This was achieved via commands on the terminal integrated with Gitpod.

### **Steps in using version control and getting ready for Deployment**

1. `git status` - would give me a list of the files which have been edited and ready for staging.
1. `git add .` - I used this command to add **all** files to the staging area instead of adding each file individually i used the `.` after `Git add` which allowed all files to be added at once, i found this workflow quicker and easier.
1. `git commit -m"Message"` - This is the command to commit the changes and the message allowed me to know what or significant changes had been made.
1. `git push` - Was used to push to the remote repository in this case **GitHub**

When working it was also neccessary to view the changes to the website, for this i mainly used preview, as the save function allowed instant refreshes and updates reflecting my changes. However for fullscreen testing in a separate tab i employed the use of the command `python3 -m http.server"` to open a port on my local machine, instructions were to make the port public then open in browser. 

_**Side note**_ I also had to become aquianted with  `git pull` and also  `git reset --hard commit-hash` as i had a problem with my project after a commit i then used the previous commands to restore my local repo from Githubs last correct commit, saving a major headache.
i then had to re push the repo back using `git push -f` 



### **How to clone or run this project natively using HTTPS.**
If you should require to fork or obtain a copy of this website you can follow these instructions. 

1. Visit my Github repo here **[MPS Repo](https://github.com/danielboots/MPS):**
1. Click on the GREEN clone or download button, located at the top right of the page see screenshot below.


    ![Repo Clone step](/images/repoclone.png)

1. Click on the "clipboard" also located on the right now seen as a dropbown box. You can either click the clipboard or the URL, if using URL method remember to right click highlighted URL and copy.
1. Open your IDE and open a new terminal window.
1. Change the directory path to a location in which you want to clone the repo too. 
1. Paste the Git URL and click ok / Clone etc. 


#### **Deploy the site to Github Pages.**
Follow these steps in order to then launch the project using Github pages to be viewed live on the web.

1. Enter the _MPS Repository_ from the Github Dashboard.

    ![GitHub Pages](/images/Repo1_pages.png)

1. Click on the settings tab.

    ![GitHub Pages](/images/Repo2_pages.png)

1. Scroll right to the bottom of the page options where you will find the "**GitHub Pages**" Options.

    ![GitHub Pages](/images/Repo3_pages.png)

From the "Source" option, chose "Master Branch" from the presented options.
The page will refresh and you will receive a notification saying. " _**Your site is published at: [https://danielboots.github.io/MPS/](https://danielboots.github.io/MPS/)**_"

___




## **Credits Acknowledgements and References.**
___
