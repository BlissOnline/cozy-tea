# cozy-tea

Tea Cozy, a tea comapny website

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

#overview
Tea Cozy is a challenge from Codecademy included in a flexbox/grid course. The purpose of this project is to leverage what I learned with flexbox

#the-challenge
-Create and mimic the site provided in the design briefing 
-Apply what I learned with flexbox

#screenshot
!-Not included 

#links 
(https://blissonline.github.io/cozy-tea/tea-cozy-main/index.html)

#my-process 
1. review the design brief to get a feel of what is needed for each section. 
  -write down stuff you'll need to learn 
2. create github repo
3. create project folder and open in VSC
4. link project to github in the git terminal 
5. organize HTML (rougly) of each section
  -create html <head> section
  -personally I like to download all photos that will be used and link the path in the html in the appriorite section
    -however I will comment the images out until I reach that scetion, the size of images can cause problems for other sections
6. create css file and link to html
7. create link to third party font if needed, or define desired font in * element 
  -make sure to include sans serif or serif backup font(s)
8. CSS start creating starting at the top and working down (This was the bulk of the work and problem solving)
  -stay on a section until it feels finished and ready to move on
  -keep responsive design in mind throughout project
9. push finished project to github
10. create readme
  -reflecting on your own expereince will deepen your own understanding 
  -this may be valuable for others working on same challenge 
  -adds value to the coding community
  -opens yourself up to more specific feedback and will help you improve faster
11. push one more time to github and than create github pages
  -use github pages to display your work on a porfolio 

#built-with
HTML
CSS (Flexbox)
github

#what-i-learned (below is a direct copy and paste of my own challenges and found solutions on every challenge I faced)
issues with connecting to github
  -I think it’s because I copied and pasted a different folders git folder
-learned inline-flex shrinks width to fit, flex value makes block level element
Challenges 
-couldn’t get 2 unique element to stay inline
  -had to nest them inside another div with the display: inline-flex
-couldn’t put items to the right
  -make container width 100%
  -be mindful of photos giving the illusion the page is bigger
-how to prevent a fixed nav bar from overlapping content below?
https://www.youtube.com/watch?v=5zDYchk3C5k&ab_channel=ByteGrad
  - body {padding-top: 60px; }to the entire body element
  - .header {top: 0;} -make sure to keep the header at the exact top
  -                {z-index: 999;}
  -                {position: fixed;}
-My super big images make it unrealistic to build prior sections
  -solution was to commit them out til I reach them, we will cross that bridge when we come to it
-how do I put text on image
  -div (img, div (h4))
  parent, display:relative (the image)
    child, display absolute (the text)
-my div background is too big 
-why is 2 different text trying to be inline 
  - make container inline-flex
    - I had to change flex-direction to column, to make items stack vertically (not sure why honestly)
-how to center the container itself
  -gave container width: 100%
  -align-items: center; 

-how do I put name under img, and center it
  -put text and img in a div
  -to center text under, text-align: center;
-how to center photo inside div
  -had to use align: items, I think because we have flex-direction: column prior 
-my elements are too big 
-how to expand photo to fit without stretching image?
  -object-fit: cover;
  -height: 100%;
  -width: 100%;
    -the percentages where messing up the overflow
-div boxes hide when srunk
  -overflow: auto
    -this will add a scroll, only when it needs to

#continued-development
-I think the fundementals of understanding the parent and child relationship is vital using flexbox
  -Tihs is an area I believe I still have to play with to gain efficiency in my workflow
-Working with images in different scenarios was challenging, I will get better and faster as I go
-Now I need to decide what to learn next, grid or dive more into javascript 

#useful-resources
https://www.youtube.com/watch?v=5zDYchk3C5k&ab_channel=ByteGrad

#author
Wes Laycock ^_^ hello

#acknowledgments
CodeCademy 

