# my-first-ticket
Challenge 1 assignment for BCU Bootcamp due 07-07-22

Contents:

1. Summary
2. Key amendments
3. Issues encountered
4. Further Questions/contributions
5. Credits

# 1. Summary

This project was undertaken as a submission for a Birmingham City Bootcamp assignment, with a brief to refactor the existing starter code with a view to improve accessibility and SEO rankings by introducing semantic HTML and consolodating CSS code where necessary.  The code style uses basic HTML and CSS.  The user story and acceptance criteria are as follows:


![Alt text](https://github.com/jonacko/my-first-ticket/blob/main/Readme_images/img_1_user_acceptance.png?raw=true "Image 1")

The image below shows the web application's intended appearance and functionality:

![Alt text](https://github.com/jonacko/my-first-ticket/blob/main/Readme_images/img_1_user_acceptance.png?raw=true "Image 2")

# 2. Key amendments

- Meaningful title
- 'Div soup'
- Image accessibility
- Consolidating CSS code
- Fixing links

### Meaningful title

I created a suitable title for the webpage (Horiseon: SEO & Online Reputation Management Services, to replace 'website' as in the source code) to make for more effective metadata.

### 'Div Soup'

On researching for the project I came across the term 'div soup' (which I love, and will now always rememeber!).  As I understand it, the 'div' elements should be used only as a last resort, and there are now (since HTML 5 was introduced) a number of more meaningful element terms to replace div that will enhance the semantic meaning of the code.  I therefore replaced the divs with the following elements (in chronological order):
- Nav
- Main
- Aside
- Footer (already assigned as a 'class' in the source code, but not an element)
- Sections within these elements

### Image Accessibility

One of the key points of the brief was to include accessible alt attributes.  I therefore included alt tags after each image source.

### Consolodating CSS code

An unnecessary number of classes were created in the source code, for example:

![Alt text](https://github.com/jonacko/my-first-ticket/blob/main/Readme_images/img_1_user_acceptance.png?raw=true "Image 3)

I therefore grouped these classes for what became the <main> and <aside> elements to make the code more efficient and easier to read, for instance:


![Alt text](https://github.com/jonacko/my-first-ticket/blob/main/Readme_images/img_1_user_acceptance.png?raw=true "Image 4")

### Fixing links

Two of the three links from the nav bar to other areas on the webpage worked using id's; I simply substituted the div elements with the anchor element to enhance the semantic meaning of the markup, and also added the link to the 'search engine optimization' text in the nav bar which was absent from the source code.

## 3. Issues encountered

1. Given that one of the key points of the acceptance criteria was to improve the accessibility of the images, I decided to add the 'hero' image using the source element in the HTML (see below), as alt tags cannot be added to 'background' images in CSS, as far as I understand.  This was the only section in which I had to keep the div elements otherwise the picture would not stretch to either far side of the web page - I did not know how to fix this otherwise.


![Alt text](https://github.com/jonacko/my-first-ticket/blob/main/Readme_images/img_1_user_acceptance.png?raw=true "Image 5")

2. After undertanking the above, I tried breaking the code in order to see if the alt tag appeared, which it did, however it changed the formatting of the other sections on the webpage and I did not know how to rectify this. All content remained the same, however.

3. After removing all the div elements and replacing with semantic HMTL elements, the <aside> section moved down the page.  I tried a number of things to fix this, such as wrapping the aside into the main and reintroducing divs.  

Eventually, I changed the 'position' of the aside section, by moving it up from the bottom by 960 px (see below), however this inevitably resulted in a large gap between the main/aside section of the webpage and the footer.  I understand this is not an ideal solution, but it was the best fix I could manage at the time...any advice appreciated!?

![Alt text](https://github.com/jonacko/my-first-ticket/blob/main/Readme_images/img_1_user_acceptance.png?raw=true "Image 5")


## 4. Further questions/contributions

1. Images in CSS/HTML - as I understand it, 'decorative' images should be included in CSS and images that relate directly to the content in HTML; I struggle to see where the line is drawn here in terms of allowing the webpage to be as accessible as possible (eg. for users with sight impairments), and feel that this particular project was ambiguous in this sense; when should images be written in HTML/CSS?

2. I am wondering whether the nav bar could be consolidated further - it would be interesting to know a) if this is possible and b) how to do this?
 
## 5. Credits

Source code: Xandromus: https://github.com/coding-boot-camp/urban-octo-telegram
