# Leah Haake's Project Worksheet 

## Project Schedule

This schedule will be used to keep track of your progress throughout the week and align with our expectations.  

You are **responsible** for scheduling time with your squad to seek approval for each deliverable by the end of the corresponding day.

|  Day | Deliverable | Status
|---|---| ---|
|Day 1 - Monday| Project Approval, Wireframes / Priority Matrix / Timeline Due, Begin Building Site | Complete
|Day 2 - Tuesday| Core Application Structure (HTML, CSS) & Working with API | Complete
|Day 3 - Wednesday| Working with API & Styling  | Complete
|Day 4 - Thursday| MVP, Bug Fixes & Deployment to Github Pages | Complete
|Day 5 - Friday| Final Touches, Update Proj Worksheet & Presentation | Incomplete

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

For my portfolio site, I would like to build a website that is simplisitic and clear. 

Use this section to describe your final project and perhaps any links to relevant sites that help convey the concept and\or functionality.

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
| Communication with Stack | H | 4hrs | 4hrs | Ongoing |
| HTML Structure | H | 2hrs | 1hr | Complete |
| Bootstrap Structure | H | 5hrs | 1hr | Complete |
| CSS Responsive | H | 3hrs | 3hrs | Complete |
| Content | M | 1hr | 1hr | Complete |
| Styling | M | 3hrs | 5hrs | Complete |
| About Page | H | 1hr | 1hr | Complete |
| Contact Form | H | 1hr | 1hr | Complete |
| Footer | L | 1hr | 0.5hr | Complete |
| Pull projects data using API | H | 3hrs | 1hr| Complete |
| Render projects data on website | H | 4hrs | 1.5hr | Complete |
| Style projects data | H | 4hrs | 5hrs | Complete |
| Setup and Deployment to Github Pages | H | 3.5hrs | 0.5 hr | Complete |
| Project previews & testing | H | 4.5hrs |  hr | In progress |
| Total |  | 40hrs| hrs |

#### PostMVP
| Component | Priority | Estimated Time | Actual Time | Notes |
| --- | :---: |  :---: | :---: | 
| Skills Section | M | 4hr | hr | Didn't work on |
| Edit Mobile Nav | L | 3hr | hr | Didn't work on |
| Add to Contact form | L | 4hr | hr | Didn't work on |
| JS/CSS Design | L | 4hr | 1hr | Added Smooth Scroll |
| Total |  | 20hrs| hrs |

-------------------------------------------------------------
## Progress Notes 

### Ideas
- For footer: change to show a hover color 
- Add CSS property to Nav items, scroll-behavior: smooth
- Look into Google Fonts and ColorHunt for styling  
- Add Text overlay on header image with my name ?

### Issues 
- Main photo - stretching when adjusting the height to rem

### Other Ideas for PostMVP
- Link to Codepen projects
- Bio image
- Image Gallery 

-------------------------------------------------------------
_Update sections below later_ 

## Additional Libraries
 Use this section to list all supporting libraries and thier role in the project. 
 -  Bootstrap

## Code Snippet

Use this section to include a brief code snippet of functionality that you are proud of an a brief description  

```
function reverse(string) {
	// here is the code to reverse a string of text
}
```

## Issues and Resolutions
 Use this section to list of all major issues encountered and their resolution.

#### Issue pushing to my GitHub repo
**ERROR**: error: failed to push some refs to 'https://github.com.lhaake/Project-1.git' Updates were rejected because the remote contains work that you do not have locally.  _My Notes:_ I think I caused this error when I was working on a new layout for my site and deleted files on my repo (such as styles.css), and the remote and local didn't match.                        
**RESOLUTION**: Stack helped me by running the command in the terminal: ``` git push origin master --force ``` 