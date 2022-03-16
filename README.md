# Escape Manchester

The Escape Manchester website is a landing page for groups and individuals to learn more about the various Escape Rooms that operate in and around the city of Manchester, UK. It offers brief details of some of the rooms available such as their difficulty, recommended group size and a link to their website.

Users are encouraged to sign up to the forum to talk to others that have a keen interest in these rooms to share their experiences and perhaps make new friends to tackle these challenges with. There are also social media links for the group and a newsletter sign up link included when registering for the forum.

![Responsive Test Image](/assets/images/readme-screenshots/responsive.png)

## UX

### Manchester Escape Rooms

Manchester offers a huge number of escape rooms that are growing more and more popular, most of which are fully booked for a full week ahead so it's safe to assume that more will appear in time to meet the demand. The goal of the website is to promote all of the companies fairly and equally to encourage users to view escape rooms they haven't yet tried and to push them towards interacting with the forums to grow a collective of like-minded teams and individuals. It also hopes to highlight the benefits of playing and offer experiences for all age ranges, group sizes and skill.

### User Stories
* As a user I want to easily find information about the escape rooms in Manchester.
* As a user I want to easily navigate to escape rooms that interest me.
* As a user I want to easily have a place to communicate with others who share similar interests.
* As a user I want a reason to return to the website.
* As the organisation we want to promote a collection of the escape rooms in Manchester in order of difficulty.
* As the organisation we want to promote mainly the escape rooms that will encourage players to keep playing.
* As the organisation we want users to interact with our forums.

### Further Planning
To plan for my project I made rough drawings of what I wanted. The site ended up looking very little to what I had envisioned in the beginning but I'm happy with the end result and glad that the site feels warm and welcoming as opposed the majority of escape room websites that are dark and gloomy to create an element of horror.

[Planning Image1](https://github.com/Samuel-Dainton/portfolio-project-1/blob/main/assets/images/readme-screenshots/project-mock1.png)
[Planning Image2](https://github.com/Samuel-Dainton/portfolio-project-1/blob/main/assets/images/readme-screenshots/project-mock2.png)
[Planning Image3](https://github.com/Samuel-Dainton/portfolio-project-1/blob/main/assets/images/readme-screenshots/project-mock3.png)

## Features

### Header & Navigation
The header features the logo and it's 3 navigational links. The logo is itself also a link back to the home page. The font changes size based on the media device size to accommodate for it's long title.
The Nav bar consists of 3 links to the index, escapes and forum pages. The 3 nav links are highlighted orange when hovered over and remain active when going to the selected link.

![Header Image](/assets/images/readme-screenshots/header-screenshot.png)

### Images
The images used are either placed in img elements or as background images through the css. I made the decisions on which they should be based on if the image worked well in its original size for different screen sizes or if it needed to scale to have a clear reason for it being there.

### Hero Image and Cover Text
The hero image changed a number of times during the creation of the site and was the major defining element in the look of the website overall. It features 4 curious explorers of an escape room and positions itself well enough across all screen sizes to give an element of mystery and theme to the website. The cover text gives a simple explanation of the site so that visitors are immediately familiar with what information to expect.

![Hero Image](/assets/images/readme-screenshots/hero-screenshot.png)

### Featured Section
The featured section is styled around the colors of the featured escape. It gives the user a video advert for the featured escape room to interact with and is followed with a positive review to encourage users into trying the escape room. Icons are used with text to give information on the recommended party size, time constraint, difficulty and the websites score for the escape. It also encourages visitors towards using the forums.

![Featured Image](/assets/images/readme-screenshots/featured-screenshot.png)

### Benefits Section
This section highlights some of the benefits of playing escape rooms and encourages readers to try them out regardless of group size or age. It uses 3 divs inside of a flexbox to position the information neatly across a variety of screen sizes, the image is resized manually when the screen size gets too small so that it doesn't overflow or push the text out of the image into the footer. 

![Benefits Image](/assets/images/readme-screenshots/why-screenshot.png)

### Footer
The footer is simple in design and features links to what would be the websites social media outlets. The icons react when hovered over by increasing in size by a ratio of 1.1 over 0.2 seconds. They also decrease in size on smaller screen sizes.

![Footer Image](/assets/images/readme-screenshots/footer-screenshot.png)

### Chose Your Adventure
On the Escapes page of the site the user first sees the hero image and text which are formatted similarly to the home page to add to the continuity of the site. An explanation for the page sits on top of or underneath the hero image of the page depending on the screen size to give users a better understanding of the following content. It again pushes interested users towards the forums.

![Map Image](/assets/images/readme-screenshots/map-screenshot.png)

### Adventure Cards
The escape room cards feature information similar to what the user will have seen on the first page and use icons to keep information simple and tight. Each of the images react when hovered over and link to the websites of the featured escape rooms in new tabs. The site rotates the cards monthly to encourage visitors to return to the website.

![Cards Image](/assets/images/readme-screenshots/adventure-screenshot.png)

### Forum Sign Up and Thank You
The forum page follows the design on the others and features a form with text, email, select and radio inputs. When submitting their information the user is sent to an identical page with a thank you message prompting them that they have been sent a confirmation email.

![Forum Image](/assets/images/readme-screenshots/forum-screenshot.png)
![Thank You Image](/assets/images/readme-screenshots/thanks-screenshot.png)

## Future Enhancements

* The adventures section is formatted to make it easy to add and remove the featured list of escapes. As the site gains more users I would increase the number of escapes listed and include ways to filter and arrange the escapes by any of their listed details such as difficulty or group size.

## Testing 

* I tested that the page works in different browsers i.e. Chrome, Firefox, Safari.
* I tested that the site is responsive and adapts to look good and function properly on all standard screen sizes using the devtools built into Chrome.
* I confirmed that all the nav elements work and that all the content is easy to read and understand using Lighthouse to score the sites accessibility.
* I confirmed that all the form entry fields are set correctly, being required where necessary and only allowing the correct type of data input, such as the email field.

## Bugs

### Solved Bugs

Clicking the Submit button on the forum page was giving me an error. I found that I needed to change the method of the form from POST to GET.

I had a lot of issues getting elements and images positioned the way I wanted with the lessons I had been taught on the course so far. I took the time to learn and experiment with flex box which solved many of the issues I had.

### Remaining Bugs

The class="logo">a doesn't inherit the text color from the body so I had to define it in the class's css.

The focus image for the hero image of the escapes page was targetting the wood background image at the bottom as well as the image and text. This was an easy fix, but for some reason moving the animation to focus on the img and text of the .wood-bg also changed the "top" property that kept the text positioned on the map correctly, so I had to go back and change all the "top" percentages for the map-text class and also all of the different media query break points.
I also noticed that using the inspection tool was making it difficult to fix this as using a view percentage of anything other than 100% would move the text.

When testing the site in Lighthouse I had a score of 77 for performance. The tool suggested fixing this by changing my larger .png files to .avif. However, doing so reduced the score to 45 even though the images aren't being flagged for their format as an issue any more.

Lighthouse recommends I change the eventListener which is in the YouTube player but I haven't found out how to change that.

## Validator Testing

* HTML
  * No errors were found when passing through the official W3C validator.

* CSS
  * No errors were found when passing through the official (Jigsaw) validator.

* Accessibility
  * I confirmed that the colors and fonts chosen are easy to read and accessible by running it through lighthouse in devtools.


### Accessibility score using Lighthouse

I managed to achieve high scores across Accessibility, Best Practices and SEO.

Performance however is affected greatly by 2 factors. 
* Lighthouse recommended I use an .avif format, this reduced the score by quite a margin and I don't fully understand why. However I did intend to keep the format as it doesn't appear to have had any noticible negative effect on any of my images. In future I intend to try using an .svg format.
* My hero images have an animation time of 3 seconds where they come into focus. Lighthouse sees this as that the text and image are unable to be interacted with and severly caps the score. So on this matter I'm not bothered, as I do believe the animation adds to the appeal of the site. 

![Lighthouse Image](/assets/images/readme-screenshots/lighthouse.png)


## Deployment

* This site was deployed to GitHub pages. The steps to deploy are as follows:
 * In the GitHub repository, navigate to the Settings tab
 * From the source section drop-down menu, select the Master Branch
 * Once the master branch has been selected, the page provides the link to the completed website.

The live link can be found here - https://samuel-dainton.github.io/portfolio-project-1/

## Credits

### Content

* The code to make the social media links and forum sign up input was adapted from the Code Institute Love Running Project.

* The focus animation, zoom on hover effect and flexbox were all learned through [W3 Schools](https://www.w3schools.com/)

* The icons used are from [Font Awesome](https://fontawesome.com/)

* The fonts used are from [Google Fonts](https://fonts.google.com/) 

* I would also like to give a big thank you to Jim, community dev for Code Institute who helped me better understand chrome's dev tools, flexbox and to get my project off to a proper start.


### Media

* [Father and Son](https://www.pexels.com/photo/a-father-and-son-giving-high-five-7005559/) 
* [Room Hero](https://wall.alphacoders.com/big.php?i=1009670)
* [Wood](https://www.wallpaperflare.com.brown-wooden-surface-background-tree-boards-texture-wooden-background-wallpaper-zzsfd/download/2560x1440)
* [Map](https://www.pexels.com/photo/beige-analog-compass-697662/)
* [Team](https://www.pexels.com/photo/photo-of-people-having-fist-bump-3228684/)
* [Detective Board](https://www.pexels.com/photo/man-in-gray-long-sleeve-suit-holding-a-pen-8369520/)
* [Desk](https://pixabay.com/illustrations/live-escape-game-live-escape-room-1155620/)

All escape room card images were taken from their respective websites.

### Final Thoughts

I feel like I would have had a much easier of a time on this project if I had all the knowledge I have gained whilst working on this project, so I'm very proud of what I have achieved and how much easier coding in html and css has become for me towards the end of the project.

Thank you for taking the time to go through my project, I hope you enjoyed it.