# **Holiday Planner** 
<img src="/assets/readmeAssets/holiday_planer_ami_image.jpg">

## Index

- [Introduction](#Introduction)
- [Project Motivation](#Project_Motivation)
- [UX](#UX) 
    - [User Stories](#User_Stories)
    - [Wireframes](#Wireframes)
- [Features](#Features)
    - [Existing Features](#Existing_Features)
    - [Future Enhancements](#Future_Enhancements)
- [Technologies Used](#Technologies_Used)
- [Testing](#Testing)
- [Deployment](#Deployment)
- [Credits](#Credits)
    - [Content](#Content)
    - [Media](#Media)
    - [Acknowledgements](#Acknowledgements)

- - - -
## **<ins>Introduction</ins>**
This is my milestone 2 project for the Fullstack Web Developer course with the [Codeinistitute](https://codeinstitute.net/). The project is not complete 
due to time constraints and the need to deploy the final version earlier than expected. I was working towards a date of the 
14th of March as per the Schedule Generator but the due date is the 05th of February. None the less the site is functional and 
has 90+% of the functions and layout envisaged at concept stage. As with my prior project I have tried to use a Agile methodology on the project and 
as such this is considered a deployment of the Minimum Viable Product (MVP), the site has the required functionality but is missing some other features that would be 
included in subsequent deployments. I will outline in the [Future Enhancements](#Future_Enhancements) sections details of the additional features 
that will be considered for future iterations.

## **<ins>Project_Motivation</ins>**
The main driver behind the development of this site was to create a holiday planner, that would become a trusted site for reviews and information on 
sites around Ireland for staycations. The site is limited Ireland, but the scope could be expanded when Covid-19 travel restrictions are eased and 
travel abroad to complete reviews is again possible. The reviews are individual and only added by the site owners so all reviews can be stood over by the
site owner, with no anonymous review information included.

As part of the design and deployment, I wanted to include two important features, the first being the ability to quickly add new locations without the need to 
recode any of the page and the second was to make the interactive map section user friendly and intuitive to use. 
The ability to add new locations quickly was achieved by placing all the location data in one file, to add a new location the location.js file can be updated with thedata for the
new location, the site picks up the new location on the next load of the page. As all the information is dynamically pick up from this file no further updates are needed. 
To make the site easy to use, the user required inputs are presented sequentially to make it easy to follow and let the user know what information they need to provide. The menus are populated 
from the locations file so only contain options when there is supporting data in the locations file. 

<img src="/assets/readmeAssets/menuView.jpg">


## **<ins>UX</ins>**
Once the concept of the site was developed, as part of the UX design phase I decided to make the site a one page site with distinctive containers for each 
section. The site would have 6 major components,

   - Header
   - Introduction
   - Destinations Information. 
   - Interactive Map
   - Form
   - Footer

Bootstrap was chosen as the main library for the major design elements, it provides the responsiveness required to ensure the site looks good and works well 
across all device sizes. On top of bootstrap, custom CSS was used to provide a unique look and feel and set the site apart. 

**Header**
The header consists of a nav bar, locked to the top of the screen as the page is long the user always has access to the nav bar to jump to the desired 
location. Under that I included a hero image with crisp white text to capture the users attention. 

**Introduction**
Consists of a short introduction to the site, some information on staycations in Ireland and a video that gives the users some media content to show case 
Ireland and holiday locations. The video is embedded as I don’t want users to leave the page at such and early stage. I decided that in this section, the 
information would be limited to generate interest but ensure the user does not get over whelmed with information and leave the site before exploring further down the page. 
 
**Destination**
To provide some more value to the users, I have included a section with some cards on major destinations and locations in Ireland. The idea here was to provide 
some information to the user if they are still deciding on the type of holiday or location within Ireland. 

**Interactive Map**
The map section is the main part of the site and as I have described above in the introduction section, this map is driven by a file with the reviewed locations 
the menus are dynamic in such that they only populate type, province & county where information to support the search is contain in the file. The file will continue 
to grow with locations. The design of the menus for the map section was set-up to guide the user through the required selections, the menus are shown when the user 
makes the previous selection and when all selections are made the button to render the map is shown. This was a design feature to make it institutive for the user. Once 
the map is rendered the user can click on the map pin, which will provide additional useful information related to the selected pin as well as the review information that is 
unique to the site.

**Form**
The form section, was included to allow site users to submit locations that they would like to have reviewed and added to the site. The thinking behind including the 
form was, two fold, first get location information to grow the site location data quickly and second, allow the user have input to the site and get invested in the sites success. 


### <ins>User_Stories</ins>

**Site User;**
- I want to find somewhere in Ireland, where I can go for my holidays. 
- I want to get additional review information on the accommodation location, outside the generic google review.
- I want to quickly link to the site of a selected accommodation if I want to book or find more information.
- A site where I can search on a wide variety of accommodation types and then narrow my search down.

**Site Owner;**
- As the site owner, I want to be able to add new locations quickly and easily without needing to update the code. 
- I want to get input from users, where do they suggest that we review and include in the site.
- Become a trusted source for reviews of accommodation


### <ins>Wireframes</ins>
Once the site concept and userstories were worked out, a wireframe was built to use as a reference guide as elements were added.
Providing a quick reference for the construction of the site during development.

| Title | Link to Wireframe (pdf) |
| --- | --- |
| Title 1 | https://app.box.com/s/c8qnumxsedgjwzw54c3bqdmbvq5oc3qe |

**Note:** There was one element added to the site that was not included in the wireframe.
A covid banner was added to the site, as the site is dedicated to travel & staycations, the banner was added as reminder to follow all current restrictions and advice.
Outside the drafted wireframe but necessary in the current Covid-19 environment.

[Index](#Index)
- - - -
## **<ins>Features</ins>**
The following section, details the existing features on the site followed, followed by a list of features to be added as enhacments or features that 
were not included due to time constraints.
### <ins>Existing_Features</ins>
- A colour palette of Black / white & Grey was used foras the prominent colours on the site with blue being used where users attention was needed for an action.
- The basic colour palette was off set with constrasting coulourfull images.
- Nav bar & footer. Minimalist design in black & white. Functional but not distracting from the site.
- Nav bar is locaked to the top of the site to give users continuious access to the links to move through the site quickly.
- Images were included as background with overlaid text, to reduce the size of the page and create visual appeal.

- Interactive Map;
    - The map is the main appeal and function of the site. 
    - It includes simple drop down menus that are populated using a locations file, this ensures only options with supporting data are presented.
    - The menus are intuitive and appear in sequence after selection to guide the user.
    - The map draws on the google maps api to populate the data based on the user selections. 
    - Pins are clickable and provide name & address data with a button for more info to click on.
    - The more info button draws data from the locations file and presents it to the user.
        - The more info functions differentiates between larger screens sizes and mobile.
        - There was place on larger screens to present the data side by side with the map, once clicked the map moves to the left
            and a table with the addtional info is presented. 
        - For mobiles, as the more info data section would be included below the map, it was decided to instead use a popup div that overlays
            the map and presents the same information but in a more mobile user friendly way.
    - The site also includes a form, this is still under construction but when completed would allow users of the site to suggest locations
        that could be reviewed and included on the site.

### <ins>Future_Enhancements</ins>
As described above in the [Introduction](#Introduction) section, there was a shorter that expected lead time to deployment.
The site was deployed and included here are a list of addtional features that were being considered if time permitted.
 - A carousel of images in the hero image section to improve visual effects on loading the page.
 - Interactive Map;
    - Upon clicking the pin, the map would zoom to the location of the selected pin.
    
 - Form Section;
    - add email service to send e-mails
    - include an responce on screen when mail is sent.
    - include a confirmation e-mail to the submitter.

[Index](#Index)
- - - -
## <ins>Technologies_Used</ins>
**Balsamiq**    https://balsamiq.com/wireframes/
- Basamiq was used in the design phase to create wireframes of the proposed web site.

**Github** https://github.com/
- Github is the repository used for version control & storage of the project.
- Github pages was used for the deployment of the site.

**Gitpod** https://www.gitpod.io/
- Gitpod was the IDE used for the development throughout the project.

**Bootstrap** https://getbootstrap.com/
- Bootstrap library was chosen for the initial layout & to provide responsiveness across devices sizes, layout was customised on top of bootstrap.

**Google Maps API** https://cloud.google.com/maps-platform/
- Google Maps API to create the map
- plotting the locations based on location data.

**Google Fonts** https://fonts.google.com/
- Google fonts provided fonts for the project (Roboto Condensed & Serrat)

**Font Awesome** https://fontawesome.com/
- Icons used through the web site are sourced from Font Awesome

**W3C Validation Service** https://validator.w3.org/
- HTML & CSS code was checked on W3C validator at the end of the project.

**HTML Formatter** https://webformatter.com/html
- HTML code was run through HTML formatter to fix any indentation issues.

**ami.responsivedesign** http://ami.responsivedesign.is/#
- The project was tested on ami.responsivedesign
- image used in readme file was taken from ami.responsivedesign site

**w3schools** https://www.w3schools.com
- For addtional code explanations & features to use.


[Index](#Index)
- - - -
## <ins>Testing</ins>
As with the previous project, I applied a DevOps type process towards development and testing. In addtiona to regular testing as features are added
and updated using, the Github http server and the responcive design mode in Firefox to simulate multiple devices. The projects was deployed to Github and 
tested on mobile devices from the github pages site. 

In addtion the following testing was carried out;

**Functional Testig**
The html codes was passed through automated code validators;
| Code | Testing | Tool | Link |
| --- | --- | --- | --- |
|HTML| Validate HTML code|W3C - Markup Validation Service|https://validator.w3.org/|
|CSS| Validate CSS code| W3C - CSS Validation Service|https://jigsaw.w3.org/css-validator/|

The inital test of the HTMl code presented erros due to the use of name tages in Anchor links, I replaced with ID tags. 
After the HTML fixes, the both the CSS and HTML code passed with no issues. 

**User Acceptance Testing**
user acceptance tesing was completed by users manually interacting with the site and checking expected functioinality vs site responce, 
in addtion the users were looking at the useability and the look and feel of the site. 

Testing was conducted on;
    Fire Fox, Safri & Chrome on Mac.
    Mobile devices, Samsung Galaxy S7 & Huawei P20 Lite.

During the course of the testing, the following bugs were found

Details of bugs found during testing
| Bug | Fix |
| --- | --- |
|White margin below footer on mobile|Issue was fixed by removing margin to the bottom of the row that was causing the white space|
|Horizontal scroll on site (both mobile & desktop|After fixing all containers and their childern to ensure that no part ran over, issue presisted. I added a section in the CSS file for body & html section to remove the overflow |
|Map menus differnt sizes on mobile|One issue reported on mobile, the menus for the map were different sizes, on desk top they were side by side and it was not an issue that they were the size of the content. Set a fixed value to improve look on mobile, where they were in a vertical row.|
|Hero image, low quality|Hero image was oigainlly added as palce holder but was not removed, testers raised issue. New image added.|
|Too much white space on the site|Users reported that there was too much white space, this was resolved by reducing the number of rows and using images as background images|
|Nav link to form lead to collapsed form|When using the nav link to jump to the form section, it was collapsed. I added JS onclick to the nav link to expand the section, nav link now takes user to the form section and its expanded.|

Time for testing was limited, to meet deployment schedule so testing was focused on testing that the website functions and that the users were not having any issues. 
The site was tested with Lighthouse on Chorme Dev tools. 

The site, did not score very highy, I did fix some issues highlighted, such as unused JS and CSS. 
I should have engaged the Lighhouse tool earlier in the development cycle.
<img src="/assets/readmeAssets/Lighthouse Test.jpg">

[Index](#Index)
- - - -

## <ins>Deployment</ins>
The project was developed using GitHub as the repository and I choose to deploy the live project on GitHub Pages,
The live site can be accessed at https://meltaylor78.github.io/holiday_planner/

**Important Note**
The main data for the locations and data that drives the interactive map are contained in the location.js file.
This file drives the menus for the map. Ensure this file remains correctly linked if you deploy the site or make a local copy of the repo.

**To complete the deployment;**
- From the Github repository 
- Navigate to the settings tab on the top of the repository page
- Scroll down to the section GitHub Pages. 
- In this GitHub Pages section, complete the deployment selection;
- Select the Branch to deploy from the first menu
    -	Select the folder from the second menu
    -	Save the settings
Further updates can be made, such as custom domain and enforce HTTPS. I did not opt for a custom domain but did select to enforce HTTPS 
for the additional security it offers. 

GitHub also provides the option to clone the repository, cloning allows you to make a local copy of the repository on your machine. 
You can complete this using the code drop down menu to get details to clone the repositor. You can find more information on how to clone a 
repository on GitHub Docs [Cloning a repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository)


[Index](#Index)
- - - -

## <ins>Credits</ins>
The developers of the Holiday Planner site would like to thank all those who contributed directly or indirectly to the development of the site, or 
through providing media and content for the site.

- - - -

| Details | Site | Link |
| --- | --- | --- |
| Discover Ireland images & video | Discover Ireland | https://www.discoverireland.ie/ |

In addtion to the list aboved, see the [Technologies Used](#Technologies_Used) and the [Acknowledgements](#Acknowledgements) section for others that we would like 
to extend our thanks and apperication to.

[Index](#Index)
- - - -

### <ins>Media</ins>

| Details | Site | Link |
| --- | --- | --- |
| Google Maps | Google Maps API | https://cloud.google.com/maps-platform/ |
| Video - Ireland – a luxury destination |  Discover Ireland - YouTube | https://www.youtube.com/watch?v=rvSdyIhpdrM&feature=youtu.be |
| Images | Discover Ireland | https://www.discoverireland.ie/ |


[Index](#Index)
- - - -

### <ins>Acknowledgements</ins>
| Name | Acknowledgement | Acknowledgement |
| --- | --- | --- |
| Rahul Lakhanpal | Project Mentor | Rahul provided the advice & input needed to develop the site. He also guided me with the layout and ascetics to ensure a modern look and feel. |
| Caroline Taylor | Content Provider | Helped to source images and content for the site. Reviewed included text|
| Caroline Taylor | User Acceptance Testing | Provided user functional testing and user acceptance testing |
| Discover Ireland | Content | For images and video content included |

[Index](#Index)
- - - -