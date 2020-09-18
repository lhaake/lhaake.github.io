# Leah Haake's Project Worksheet 

## Project Schedule

|  Day | Deliverable | Status
|---|---| ---|
|Day 1 - Monday| Project Approval, Wireframes / Priority Matrix / Timeline Due, Begin Building Site | Complete
|Day 2 - Tuesday| Core Application Structure (HTML, CSS) & Working with API | Complete
|Day 3 - Wednesday| Working with API & Styling  | Complete
|Day 4 - Thursday| MVP, Bug Fixes & Deployment to Github Pages | Complete
|Day 5 - Friday| Final Touches, Update Proj Worksheet & Presentation | Complete

##  Research 
Spend sometime and look at a few portfolio  and/or web sites to find some design or functionality that you would like to incorporate into your own portfolio.  Record those findings below:

Link To Site  | One Thing I'd Like To Incorporate | 
| ------------- | ------------- |
| [https://www.lianapenn.com/](https://www.lianapenn.com/)| Skills section
| [http://andrewhollingworth.com/](http://andrewhollingworth.com/)| Footer design
|  [http://eloise-ress-barrow.surge.sh/#projects-header](http://eloise-ress-barrow.surge.sh/#projects-header)| Projects section and contact page. I also like that in the mobile view the nav shows initials "erb"
|  [http://helloaileen.com/#contactWrapper](http://helloaileen.com/#contactWrapper)| Homepage image with name and web developer text overlay
| [https://angelolsen.com/whole-new-mess/](https://angelolsen.com/whole-new-mess/)| I like the Nav and typeface 


## Project Description

For my portfolio site, my goal was to build a website that is simplistic, clear, readable, easy to use and meets the requirements. 

## Google Sheet

My [Google Sheet](https://docs.google.com/spreadsheets/d/1GozbvSSln3rtpnqxqOF7xpyThqbDv532YxUGB41sd5o) 

## Wireframes

- [Mobile](https://res.cloudinary.com/lhaake/image/upload/v1600031129/Project%201%20Wireframes/Mobile_Version.png) The mobile version shows a hamburger menu for the nav, the projects stacked to display 1 per row. 
- [Tablet](https://res.cloudinary.com/lhaake/image/upload/v1600031136/Project%201%20Wireframes/Tablet_Version.png) The tablet version shows the regular nav, the projects displaying 2 per row. 
- [Desktop](https://res.cloudinary.com/lhaake/image/upload/v1600031143/Project%201%20Wireframes/Desktop_Version.png) The desktop version shows the regular nav, the projects displaying 3 per row. 


## Time/Priority Matrix 

- [List Link](https://res.cloudinary.com/lhaake/image/upload/v1600032269/Project%201%20Wireframes/Priority%20Matrix%20List.jpg)
- [Graph Link](https://res.cloudinary.com/lhaake/image/upload/v1600032257/Project%201%20Wireframes/Priority%20Matrix.jpg)

### MVP 

- Project Approval, Meetings & Communication with Squad Lead, Stack
- Building HTML and CSS Structure for Mobile (first), Tablet and Desktop
- Organize Site Content, including the text, any images
- Styling (color and font choices)
- Use Bootstrap
- Nav 
    - Mobile - Hamburger Menu
    - Tablet & Desktop versions
- About page 
- Contact form
- Footer and social media icons
- Working with API 
    - Update projects content on google sheets
    - Pull data using google sheets api
    - Render data on page 
    - Styling
- Project previews and testing 
- Setup and Deployment to Github Pages 


### PostMVP 

- Skills section (programming langauges and technologies)
- On Mobile Nav, edit name to show initials 
- Add drop down or radio buttons to Contact Form
- Additional JS/CSS Design or Animation


## Functional Components 

#### MVP
| Component | Priority | Estimated Time | Actual Time | Status |
| --- | :---: |  :---: | :---: | :---: |
| Communication with Stack | H | 4hrs | 4hrs | Complete |
| HTML Structure | H | 2hrs | 1hr | Complete |
| Bootstrap Structure | H | 5hrs | 1hr | Complete |
| CSS Responsive | H | 3hrs | 6hrs | Complete |
| Content | M | 1hr | 1hr | Complete |
| Styling | M | 3hrs | 4hrs | Complete |
| About Page | H | 1hr | 1hr | Complete |
| Contact Form | H | 1hr | 1hr | Complete |
| Footer | L | 1hr | 0.5hr | Complete |
| Pull projects data using API | H | 3hrs | 1hr| Complete |
| Render projects data on website | H | 4hrs | 2hr | Complete |
| Style projects data | H | 4hrs | 5hrs | Complete |
| Setup and Deployment to Github Pages | H | 3.5hrs | 0.5 hr | Complete |
| Project previews & testing | H | 4.5hrs |  2hr | Complete |
| Total |  | 40hrs| hrs | |

#### PostMVP
| Component | Priority | Estimated Time | Actual Time | Notes |
| --- | :---: |  :---: | :---: | :---: | 
| Skills Section | M | 4hr | hr | Didn't work on |
| Edit Mobile Nav | L | 3hr | hr | Didn't work on |
| Add to Contact form | L | 4hr | hr | Didn't work on |
| JS/CSS Design | L | 4hr | 1hr | Added Smooth Scroll |
| Total |  | 20hrs| 1hr | |

-------------------------------------------------------------
-------------------------------------------------------------

## Additional Libraries
 -  jQuery - JS Library
 -  Bootstrap - CSS Library
 -  Font Awesome - Icon Library

## Code Snippet

Working on the render function involved applying different concepts we covered in week 1 and 2 about objects, function expressions, arrays, array methods and jQuery. 

- I spent some time making sure I understood how the data was being passed into render() from the return statement and that it was an array of objects, and would need to grab the object keys using dot notation. Using a forEach() method would be good for iterating over the array. 
- I visualized appending the data on the page in steps that built on one another. 
    - Creating a div, then creating a h3, p and img tag to place in the div
    - Adding the div to the article element
    - Grabbing the data from Google Sheets and adding to particular elements (h3, p, img)

```
// Create function that adds Projects to DOM

const render = (projectsArray) => {
    console.log("Testing the projectsArray", projectsArray)

    // Using forEach() to append each project to page 
    projectsArray.forEach((project, index) => {
        // create new HTML elements and store in variables 
        const $projectDiv = $("<div>");
        const $titleText = $("<h3>");
        const $descriptionText = $("<p>");
        const $img = $("<img>");

        // append HTML elements to the div
        $projectDiv.append($titleText);
        $projectDiv.append($img);
        $projectDiv.append($descriptionText);

        // add a class to the div 
        $projectDiv.addClass(`proj-div-${index}`)

        // add the div to the article and a new class to article
        $("article").append($projectDiv).addClass   ("projects-container");

        // Append the projects data .title, .image and .description to the speciifc HTML elements
        $titleText.append(project.title).addClass(`proj-title-${index}`);
        $img.append(project.image).attr("src", project.image).addClass(`proj-img-${index}`);
        $descriptionText.append(project.description).addClass(`proj-description-${index}`);

        console.log(project);
    })
}

```

## Issues and Resolutions

#### Issue 1: pushing to my GitHub repo
**ERROR**: error: failed to push some refs to 'https://github.com.lhaake/Project-1.git' Updates were rejected because the remote contains work that you do not have locally.  _My Notes:_ I think I caused this error when I was working on a new layout for my site and deleted files on my repo (such as styles.css), and the remote and local didn't match.                        
**RESOLUTION**: Stack helped me by running the command in the terminal: ``` git push origin master --force ``` 

#### Issue 2: Creating unique classes in render() function 
**ISSUE**: My issue was I wasn't sure how to target a specific item in my ProjectsArray while using the forEach() array method. I'm familair with targeting array items using bracket notation and a loop counter variable [i]. I wanted to be able to add unique classes to my project data (div's, images, etc) on my page and could style them individually.               
**RESOLUTION**: Stack helped me by sending a [MDN article](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) about the forEach() array method, and that I could use string interpolation to create these classes for each item in the array.  


### Future Direction & Ideas
- Links to my Codepen projects
- Polish my projects
- Add to my About section, maybe include a Bio photo
- Try out bootstrap cards for styling projects
- Create the CSS Grid Image Gallery pproject with my own photographs
- Work on the contact form functionality 
- Resolve Issue: Edit the header photo - stretching when adjusting the height so that the image doesn’t take up so much space. I may add an overlay of transparency or text on the image. 
