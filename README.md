
# Taekwondo Migration Guide

Welcome to my first proyect of [Code institute](https://codeinstitute.net)!

As part of the first project for my training as a Fullstack Developer, I have developed this project that allows me to develop an idea in relation to the change of martial arts practice to facilitate the learning of a new style or practice, building on previous knowledge of a known practice. At the same time, it allows me to put into practice what I have learnt about coding/layout in my training as a Fullstack devoleper in the [Code institute](https://codeinstitute.net) training programme.

![Gallery Example](https://github.com/patchamama/PP1-Taekwondo-Migration-Guide/blob/main/doc/screen-shot-responsive.png)

## The goal

The idea of this guide is to facilitate the learning of a martial art starting from an already known martial art and for this point, we start by looking for an equivalent to every position, strike or block between a known martial arts and the target of learning. In general there are always subtle differences (even in these techniques within the styles of the same martial art) and I do not want to find an exact approximation but an idea that allows us to use a known martial art as a reference and from there make modifications and achieve the final technique in the new martial art that we want to learn and thus facilitate rapid learning and adaptation to the new practice.

## Features

To achieve the objectives I have divided the project into 4 main pages/sections that are included in the menu that is displayed on each page and that always allows you to access them from wherever you are on the site.

### Sections common to all pages

- __The landing page image__

  - Three images are included in a salute sequence as part of the martial philosophy of these arts, which are mainly based on the unity and balance of body and mind control.

- __Menu Bar__

  - It includes access to 4 different pages: home, migration, gallery and contact. The menu is displayed on every page, so it is accessible from any section of the page and avoids the use of backtracking options.   

![Landing Page and menu bar](https://github.com/patchamama/PP1-Taekwondo-Migration-Guide/blob/main/doc/menu-landing-page.png)

- __The Footer with medialinks__ 

  - It is possible to provide the link in the future to the different social networks of the association to which I belong once I provide this information by the coordinators (the information has not been provided). 

### Page-menu: Home

- __Why this page?__

  - In this section I specify the reason for the content of this page with a brief history and the initial difficulty that determined learning a new martial arts practice without a guide that would allow a quick transition and clarification of the new concepts.

- __Introduction__

  - The introduction briefly gives some general concepts such as the meaning of martial art and gives more information about the diverse origin of martial arts and possible causes. 

### Page-menu: Migration

  - This is the most important page of the project. A comparative table summarises the equivalents between Korean, Japanese and Chinese martial arts (respectively taekwondo, karate and kungfu) in different techniques of basic stances, striking and blocking techniques. Each practice is specified in a different colour to make it easier to differentiate the content on small screens as the full table cannot be displayed.
  - This has been the biggest challenge of the project, because in addition to the value of the content, it was desired to present the content from the beginning in a comparative table. After achieving 4 tables, the possibility of displaying them correctly on all devices (responsive) was a problem, so the solution was separated into several ideas:
    - To convert the 4 tables into one table in order to achieve uniformity in the columns without depending on the size of the contents,
    - Convert the tables for use with containers ( table > divs ) and so in this way, can be changeg the table format to blocks in different lines, differentiating the content with different margins and different colours,
    - In the last instance, due to the length of the content on small screen devices, a text was added to each cell to clarify the language of the practice to serve as a additional reference to the colour.

![Table big](https://github.com/patchamama/PP1-Taekwondo-Migration-Guide/blob/main/doc/table-big.png)

![Table small](https://github.com/patchamama/PP1-Taekwondo-Migration-Guide/blob/main/doc/table-small.png)

### Page-menu: Gallery

  - The gallery includes sample images taken from [Pexels](https://www.pexels.com/) which should be replaced in the future by images from the association.

![Gallery Example](https://github.com/patchamama/PP1-Taekwondo-Migration-Guide/blob/main/doc/gallery-sample.png)

### Page-menu: Contact

  - In the contact section there is a reference to the association I am part of with a small reference to the types of training they do. The information was taken from the association's website. There is a contact email, postal address and a link to google maps for more detailed information.

### Features Left to Implement

  - Video session showing each technique and the differences between each one.

## Testing 

  - Several tests have been carried out to check that the website contains as few errors as possible:
    - The display of the page has been checked on several devices (android phone and tablet, iPad and a laptop Macbook Pro with different browsers: safari, chrome, edge and firefox in their current versions and no error or change of behaviour on the page has been appreciated. Only one bug has been found in the header animation in Safari which is specified in the next section.
    - It has been checked that the page is responsive on different screen sizes (devtools in chrome vers. 111.0.5563.64) and has worked as expected.
    - No errors have been detected in the official html validator: [W3C validator](https://validator.w3.org/nu/?doc=https://patchamama.github.io/PP1-Taekwondo-Migration-Guide/)
    - No error has been detected in the official css validator: [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https://patchamama.github.io/PP1-Taekwondo-Migration-Guide/&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css)
    - Performance tests were done using lightouse (devtools) in chrome and the data returned is quite good.

![Performance results](https://github.com/patchamama/PP1-Taekwondo-Migration-Guide/blob/main/doc/performance.png)


### Unfixed Bugs

It has been detected that in Safari version 16.3 sometimes the animation does not work on a MacBook Pro (MacOsx Ventura) and due to the lack of availability of another Safari on a different computer it has not been possible to check if the problem is specific to my computer (for some plugin or other reason). However, in Safari on a 9 generation iPad the animation of the page header works perfectly.

## Deployment

The project has been completely developed based on a template from the [Code Institute](https://github.com/Code-Institute-Org/gitpod-full-template) in github and after the replication, gitpod has been used as an online IDE that allows updates to be made in github. To deploy the application, got here to the "Settings" section over right > left menu "Pages" and from here you can access directly to the link: https://patchamama.github.io/PP1-Taekwondo-Migration-Guide/ 
To the html and css formater was using: https://codebeautify.org/

## Credits 

- All content was extracted directly after consultation with [chatGPT](https://openai.com/blog/chatgpt) and by checking the information obtained directly with my experience as a practitioner of karate, hapkido and taekwondo. In the case of Kungfu it has not been possible for me to check the validity of the information.
- The information on the contact page has been taken from the website of the [Ho-Sin-Sul-Berlin e.V. Hapkido Verein](http://www.hosinsul-berlin-ev.de/training/)
- The images in the gallery section and the header were taken from the site: https://www.pexels.com/
- To make the tables responsive, I converted the original html table tags (table, tr, th, td...) into divs and based it on the idea of the site: https://divtable.com/converter/
- Animation of logo using a idea of https://stackoverflow.com/questions/69436632/css-keyframe-animations
- The idea of inserting a text in a container (div) via css without using javascript was taken from the site (for the table in the migration section on small screens): https://stackoverflow.com/questions/2741312/using-css-to-insert-text
- Menu Icons and sections are from: https://fontawesome.com/
- As part of the learning and test-error process, much of the knowledge practised here is a result of the exercises and ideas learned in the [Code institute](https://codeinstitute.net) training period and adapted to my needs.

All photos are open source licensed.
