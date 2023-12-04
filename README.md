# DCIT_205_IA

NANA ESSENEY MEWIEDELA YENTUMEY
11339613
DCIT205 IA DOCUMENTATION

<hr>

#INTRODUCTION AND PURPOSE

Welcome to my repository for the University of Ghana Computer Science Department website. 

This project aims to provide a robust and user-friendly online platform tailored to meet the unique needs of both students and faculty members within the department.

The primary objective of this codebase is to create a dynamic and interactive website that serves as a central hub for information, communication, and collaboration within the Computer Science Department at the University of Ghana. 

From academic resources to departmental announcements, event calendars, and timetables for various levels, this website is designed to streamline communication channels and enhance the overall experience for both students and faculty.

<hr>

KEY FEATURES

•	Dynamic Home Page: Get easy access to all the most important parts of the website right on the homepage.

•	About: Get useful information about the department and its components to help you make an informed decision in anything regarding joining or participating in the activities of the department.

•	Programmes: Get detailed information about the various courses our department has to offer to better decide the kind of future you want for yourself.

•	Resources: Access our social platforms, student handbook, and other educational resources.

•	Event Calendar: Keep track of departmental events, seminars, and important dates.

•	Student timetables: Get easy access to the class timetables of department members as well as the general academic calendar to help you plan out your year properly.

<hr>

#HOW TO CLONE AND SET UP THE PROJECT:

Step 1: Visit https://github.com/death-inspires-me/11339613_DCIT_205

Step 2: Click the "Code" button

Step 3: Copy the link provided in the pop up menu

Step 4: Open your git bash and type in the command "git clone (url copied) (folder you want to clone the repository into)"

You can also choose to download the zip folder from the pop up menu and extract it's contents into the folder of your choice.

<hr>

My project consists of ten HTML webpages:

1.	Home

2.	About

3.	Programmes Offered

4.	Short Courses

5.	Undergraduate Courses

6.	MPhil/MSc Courses

7.	PhD courses

8.	School and Class Timetables

9.	Department Events

10.	Resources for Department Events

One CSS file:

1.	main.css

Two JS files:

1.	header.js

2.	collapsible.js

All HTML files are linked to main.css and header.js in the head section for styling and the behaviour of the header but only undergraduate.html, phd.html, and mphil.html are linked to collapsible.js for the collapsible lists.

All files except home.html have a style element in the head section that determines the page background and behaviour in CSS.

<hr>

BASIC STRUCTURE:

Every page consists of four main visible parts:

1.	The navigation bar

2.	The header

3.	The body

4.	The footer


The font-family used throughout the project is “'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;”

The scroll bar of every page is also styled with a minimalistic blue bar using the body::webkit-scrollbar embedded class in CSS.

The thematic colours of the whole site are white, #153d6f, and #bd9c6c.

I also included a stylistic choice of background blurs and rounded corners for media and outlined sections for various "div" and "main" elements within the code base to add a modern feel to the page. The CSS properties that make that possible are “backdrop-filter: blur(10px);” and “border-radius: 8px”.

You will also find many sections given a white outline with the outline-style: groove. This is to provide a proper distinction between different parts of the page and enhance visibility since all the sections with blurry backdrop filters have no background or in CSS: background: none;

The resources for all styling choices such as images, videos, and icons (which can be in both .png and .svg) are found within the same folder as the HTML files.

Logos and icons used were mostly sourced from https://fonts.google.com/icons.

<hr>

1.	THE NAVIGATION BAR

The navigation bar is created with the HTML element "nav" with the class “navbar”.

Each button on the navigation bar is a list item (with class “nav-item”) within an unordered list (with class “navbar-nav”).

This includes the school logo (with class “logo”) at the very top which is just an image link to the university’s main website rather than an actual button.

Every "button" element is within a "div" element and every button ends with a "span" element that gives each button a tooltip that describes what the button is for to the user on the webpage.

The navbar class is given a transition property for a small animation when it’s hovered upon and a z-index property with a value of 100 to make sure it appears above everything else on the webpage no matter what. 

The hover animation on the navigation bar is done using the transition: property with a time value of 200ms.

Finally, each button button on the navigation bar also has tooltip to allow the user to know what the icon does without having to click on it.


2.	THE HEADER

The header is a div with class “header”.

The header class is given a z-index value of 50 to make sure it appears above everything else on the webpage except the navigation bar.

Everything contained within the header is contained within a div with its own class and every component of the header is styled and positioned individually.

JavaScript code is added in the header.js file to make the header stick to the top when the user scrolls down.


3.	THE BODY

The body of the home page has a looped silent video (with a video" element and an id “myVideo” for a background). 

The video is given a few properties to make sure it displays under the whole page and a z-index value of –1 to make it appear only below every other component of the page no matter what.

All other pages apart from the homepage have a static image for a background using a background: fixed; property to make the page’s content move over the image rather than having the browser duplicate the image repeatedly to fit the contents of the page and a background-image: url() property to determine the image used.   

The styling for the background of other pages is in the head section of their HTML script.

The various main sections of each page are placed within a "main" element which is styled with an outline and a blurry backdrop.

An "hr" element is added in some cases to distinguish between sub-sections within the main sections.  

Sections within which elements are to be displayed side-by-side are usually given a display: inline-flex; property or a float: left/right; property to make the positioning of the elements less manual although manual adjustments are needed in some cases.

Finally, to create a smoother and more unique feel, most sections with outlines are given rounded corners using the border-radius: 8px; property. 


4.	THE FOOTER

The footer section which is at the bottom of every page and forms the entirety of the help and support page created using the "footer" element. It is styled the same as the main sections.

However, it consists of unordered lists ("ul") of links to various helpful sites placed side by side.

<hr>

OTHER IMPORTANT INFO:

•	The PDF files embedded in the home page and on the timetables page are done using the "object" element with a data attribute giving the source for the file and a type attribute describing the type of file as application/pdf.

•	The collapsible lists used in the undergraduate, MPhil, and PhD pages are buttons (with class “collapsible”) within divs connected to unordered lists also within divs (with a class “content”).

•	Each page with a collapsible list button is linked to the collapsible.js file using the "script" element which contains JavaScript code that makes the list appear on-click based on the length of the list and number of list items to make sure every item in the list appears fully.

<hr>

#SCREENSHOTS:

1.	Home page
       
![Screenshot of homepage](/Screenshots/ss%20home%201.png)
![Screenshot of homepage](/Screenshots/ss%20home%202.png)
![Screenshot of homepage](/Screenshots/ss%20home%203.png)
![Screenshot of homepage](/Screenshots/ss%20home%204.png)
![Screenshot of homepage](/Screenshots/ss%20home%205.png)
![Screenshot of homepage](/Screenshots/ss%20home%206.png)
![Screenshot of homepage](/Screenshots/ss%20home%207.png)


2.	About Page

![Screenshot of about page](/Screenshots/ss%20about%201.png)
![Screenshot of about page](/Screenshots/ss%20about%202.png)
![Screenshot of about page](/Screenshots/ss%20about%203.png)
![Screenshot of about page](/Screenshots/ss%20about%204.png)
![Screenshot of about page](/Screenshots/ss%20about%205.png)


 3. Programmes Offered

  ![Screenshot of programmes page](/Screenshots/ss%20program%201.png)
  ![Screenshot of programmes page](/Screenshots/ss%20program%202.png)

4. Short Courses page

![Screenshot of short courses page](/Screenshots/ss%20shortcourses%201.png)

5.	Undergraduate courses page
    
![Screenshot of undergraduate page](/Screenshots/ss%20undergrad%201.png)
![Screenshot of undergraduate page](/Screenshots/ss%20undergrad%202.png)
![Screenshot of undergraduate page](/Screenshots/ss%20undergrad%203.png)
![Screenshot of undergraduate page](/Screenshots/ss%20undergrad%204.png)

6.	MPhil/MSc courses page

![Screenshot of mphil page](/Screenshots/ss%20mphil%201.png)
![Screenshot of mphil page](/Screenshots/ss%20mphil%202.png)
![Screenshot of mphil page](/Screenshots/ss%20mphil%203.png)
![Screenshot of mphil page](/Screenshots/ss%20mphil%204.png)

7.	PhD programmes page

![Screenshot of phd page](/Screenshots/ss%20phd%201.png)
![Screenshot of phd page](/Screenshots/ss%20phd%202.png) 
![Screenshot of phd page](/Screenshots/ss%20phd%203.png)  

8.	School and Class timetables Page

![Screenshot of timetables page](/Screenshots/ss%20timetables%201.png) 
![Screenshot of timetables page](/Screenshots/ss%20timetables%202.png) 

9.	Department events page

![Screenshot of events page](/Screenshots/ss%20department%201.png)
![Screenshot of events page](/Screenshots/ss%20department%202.png)


10.	Resources page
   
![Screenshot of resources page](/Screenshots/ss%20resources%201.png)
![Screenshot of resources page](/Screenshots/ss%20resources%202.png)

<hr>

#WHAT I HAVE LEARNED FROM THE PROJECT:

I improved my knowledge of front-end technologies and obtained insightful knowledge about web development. 

I also learned the value of semantic markup for accessibility and SEO while creating the HTML structure, and CSS helped me improve the sites' appearance and organisation. 

By using JavaScript, i gained knowledge of how to add dynamic functionalities to for enhancing user interactions of a webpage. 

Whenever I ran across difficulties with responsive design and cross-browser compatibility, debugging and problem-solving became second nature to me. 

The project placed a strong emphasis on the value of collaborative workflow, organised code, and efficiency. 

In summary, this experience broadened my knowledge of web development concepts, building a strong basis for upcoming work and enhancing my ability to design interesting and useful websites.