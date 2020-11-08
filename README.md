# Audio-Phonics-Product-Landing-Page

Responsive Web Design Projects - Building a Product Landing Page. Using HTML and CSS to complete this project.

The goal is to create a responsive product landing page for headphones, modelled after Senheiser Headphones. Since this project is also a part of the 100daysofcode challenge all of the additional notes for it will reside in the 100 days of code repository which I have forked. File to look for > log.md. 

#Day 7: November 3, 2020 



**Today's Progress**: Started a new project, a product landing page for Audio-Phonics headphones.

**Thoughts:** 

HTML and INTRO

Creating a product landing page, for headphones, with lightbox gallery and submit form. Deploy it to Netlify.
We’ll have a navbar, showcase area, dark overlay area and a photo gallery with grid and lightbox (simple lightbox). In the footer we’ll have menus, email subscribe form.

Bringing on the css and js from lightbox. Using Google Font Catamaran.

IMPLEMENTING AJAX GOOGLE APIS
ADDING A jQUERY SCRIPT 

Implemented the Ajax.googleapis.com so we could run the simple-lightbox.min.js file with our gallery and links.
And the script function is a line of jQuery. jQuery is a JavaScript library designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax.

CREATING THE NAVBAR

Created the navigation bar with hash links and added the id to body so when we click the home link.

ASSIGNING ROOT COLORS

CREATING OUR RESETS

Box sizing to border  box, so that padding and boarders don’t ad width to the element. Zeroing out the margin and padding.

BASE STYLES

For the body we’re setting the font family, line height, color and font size.
Headings will have a different line height.
Links will have a custom properties color and a text decoration of none so there’s no underline.
From the unordered list we take away the bullet points with list style set to none.
For any image we have on this site we want it to take a 100Q% of the width of the container.

CREATING THE CONTAINER CLASS AND GRID SYSTEM

We’ll be creating the container class and we’re also going to use the grid system to align the logo on the left and the menu on the left. 

For the container we’ll set the max width 1100px which is pretty common and margin auto so it gets put in the middle and here’s even margin from the left and right. 
Overflow will be hidden because we don’t want anything breaking out of the container. 
Padding will be set to 0 from top and bottom and 2rem from left and right.

STYLING THE NAVBAR 

We don’t want to display grid on the navbar class, because if we do that then the container is going to be the grid item but we want to display the H1 and the UL as our two grid items. Setting the display to grid for the navbar container and specifying the way the space will be laid out, 1fr and 1fr or repeat

SHOWCASE AREA

We’re going to us a section and give it a class of section-a and have a DIV with a container underneath to push everything in the middle just like with the navbar. Another DIV with H1 and Paragraph and an anchor link with a button class underneath. 
Under the DIV we’ll have an image showcase.jpg

MAKING THE GRID LAYOUT

We want to display the grid on the container not on the section-a because when we do it on section-a the container will be the only grid item but we want two.
Now were’ creating a section-a separately because we want to add some margin top and bottom. We could also create some utility classes for margin, padding if we’d want like we did with the previous project but we’re keeping it simple.

On the container we’ll set the display to grid and grid template-columns to repeat 2 1f
Creating a small grid gap and now with align-items and justify-content set to center we’ll center everything 

Also, we added a bit of margin to the navbar because the photo of th headphones is touching too close to the Home and About.

We added a font-size to the section-a H1 and a color from the custom properties.
And section-a paragraph got a margin top of 1rem to help spread it out a bit more and a fon-size of 1.2 rem to help the text be more evenly distributed.


**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 8: November 4, 2020 



**Today's Progress**: Creating the overlay section and gallery.

**Thoughts:** 

STYLING THE BUTTON 

We’re using display as inline-block so we can add width and padding. It doesn’t take up its own line compared to block items. Don’t forget to add a cursor pointer and change the font size to match the purpose of the page. For a product landing page, we’re making everything a bit bigger to make it stand out. And of course the border radius and here we’re going strong with this one to match the curves of the headphones as well.
We’re also setting the button hover to be a bit different so it’s noticeable when clicking.

CREATING THE OVERLAY SECTION

Let’s add the markup for that first and we’re breaking everything up into sections. Adding a div with the class overlay and in that one a section-b with H3 and H2 and a paragraph.

OVERLAY TEXT

So, with section b’s CSS we’ll position it relative, because we’re going to position the overlay absolute withing section-b and since section-b is its container it needs to be positioned relative. And this is where we’ll add the image as our background ../img meaning up one level to the img folder. Adding no repeat, so it doesn’t repeat, positioning bottom center and cover the whole space. We’ll set the height of the img to 600px.

Position is set to absolute withing the section -b or within wrapper is relative. Top 0, left 0 so the top left corner (remember how you learned about the square positioning with Angela Yu, this is it). And we want it to expand a 100% height and also a 100% width. So it cover ther whole area. Setting the background color to rgba which comes from our custom properties color. We can also change the color opacity as the last value of the rgba.

SECTION B TEXT
Setting the color to white and set the height 100% of its container. We’re using flex, however I don’t want it to be aligned horizontally, so we want to change the flex direction to column. We want to align everything to the center with algin items and justify content and text align

CHANGING THE SIZE OF THE TEXT

We canged the h3 font size to x2 larger. The h2 fon size to a whopping almost x5 larger and added margin top
With the paragraph we made it a bit bigger and added some padding as well.

THE GALLERY

We’re making a section-c and but not using a container because we want it the gallery to go from end to end. Gallery is going to be our GRID container and then we’re going to have links with images. Using a link to our image, and a class BIG which is part of the simple lightbox and we have the location of the image.

Now we want to target each picture and modify the grid so that they all span across and take up room appropriately. We don’t need to give them all classes because we can use pseudo selectors like first child to assign them properties. We can do it this way or there’s a shorter way as well. This means that we’re assigning the picture to start from the edge and take up rows 1-3 and columns 1.3

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 9: November 5, 2020 



**Today's Progress**: Working on adding the lightbox feature and making the footer also adding media queries.

**Thoughts:** 

CREATING THE LIGHTBOX

Creating the lightbox turned out the be easier than expected. Instructions from the developer Andre we’re simple and structured. Added the dist folder wit the simple lightbox css and js files. Added a link to my markup regarding css and a script at the bottom regarding js. I’m so happy that it turned out looking great.

CREATING THE FOOTER

First we’re creating a section footer class with the footer tag. Then We’ll proceed to add a container DIV which will have grid items inside.

Now, we’re adding in two more grid items which will be Company info and Blog Post. Each will have a list, first one will have an unordered list and list items, second one will have just list items.

We’re adding another grid item with the heading of Subscribe and a paragraph. Now we’re entering a form with a name of email-form , method POST for it to work and an attribute of data-netlify and set that to TRUE and that’s how we can use their form submission system.
Now, we’re going to have a new div with a class of email-form in order to style the form and then a span with a class of form-control-wrap and in that span is where will have the input. We also added a button with a type of submit and a class and added an icon from font awesome.

We’re targeting the section footer and assigning it a background color from our custom properties and a text color of white. Also, some padding of 4 rem

Now moving on we’re targeting the container itself and setting the display to grid and grid template columns to 4 equal 1fr’s and a grid gap of 1rem.

Added attributes to the headings and also to the links. Went back and wrapped the Blog post list in <ul> tags so it would get rid of the bullet points.

Now, we’re targeting the section footer links that have the i tag in them. We used similar targeting in the previous project but I need to practice it more. 

The idea is to move the submit over to the right, we’re positioning it absolute withing the email form which is positioned relative. And we’re making the width and height 45px and we’re moving it to the top and right, so we’re moving it over as we can see compared to where it was first. 

Background color change, padding and margin 0 and we want the rounded corners on the right and bottom
 
ADDING MEDIA QUERIES 

Now we want to have the headphones come first so we need to target the first element which is the DIV in the section a with the text and put that in the second place and image in the first place. We can use pseudo selectors to achieve that.

Modified the footer to be in one column with 1fr and text in the center and also set display to none regarding the company name and blog post columns so it would look more minimal.

NETLIFY FORM

DEPLOYING TO NETLIFY

Pushed my project to GitHub and then deployed in Netlify https://audio-phonic-product-landing-page.netlify.app/.


**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 10: November 6, 2020 



**Today's Progress**: Debugging the footer email form

**Thoughts:** 

I knew what I wanted to do today but I didn’t expect for it to be this difficult, let me explain. Although I finished the Audio-Phonic’s product landing page yesterday, I noticed that when I deployed it to Netlify and checked it out on my mobile (iOS) the email form wasn’t appearing in the footer column. 

It was already late yesterday evening and I set a goal for today, that instead of starting with a new project I’d spend a day, or however long it took to figure out what the issue is with the footer. So, around comes today and I’m excited to get going on the debugging and it just ain’t happening, I mean I’m new at coding, fresh, but from todays experience I can tell that it’s even more difficult to debug something than code. 

I knew where the problems was but to pinpoint it is another matter entirely. Did the fix work, yes, eventually and I got the form back on the mobile portrait layout as well. Is the bug fix working exactly like I want it to, no, not yet and I’ll continue working on that tomorrow. 

I want to understand how using .section-footer div:nth-child(2) and .section-footer div:nth-child(3) exactly makes my form disappear just on the Netlify platform, because I had it deployed on GitHub pages as well and its visible there. Am I content, no. 

Am I closer to being content, definitely but I just need to get the page working the way I want it to operate and then we’re good to proceed on to greener pastures.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)


#Day 11: November 7, 2020 



**Today's Progress**: Debugging the footer email form a bit further

**Thoughts:** 

Found the fix for the footer email form. I added a class to the form tag and styled in CSS with display flex and flex-direction column. It worked in placing the email form at the bottom of the footer in Netlify.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)