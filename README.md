# Horiseon-HTML-CSS-Refactoring

## Description

The purpose of this project is to make the existing code more "beautiful" without changing the Horiseon website's functionality. By creating this repo, I am hoping to solidify my understanding of CSS and HTML by improving the structure of the existing code and readability. By increasing the readability and efficiency, this website's code will be easier to maintain. 

What I learned:

- How to apply semantic elements (Header, body, main, section, aside and footer)
- How to spot repetitive styling and use IDs/define variables to make the code more efficient/cut down unnecessary code lines

What I did:

HTML
- Explored the website to get familiar with the look and functionality of the site
    - Noticed the 'Search Engine Optimization' nav link/button was not functioning like the other two buttons when clicked
        - Missing id="search-engine-optimization" on line 29 (added this - fixed issue)
- HTML file is flooded with divs
    - Replaced div tag on after head and before html tags with the body tag

    - Replaced div tag that encapsulates the h1 and ul with the header tag

    - Replaced div wrapping ul with nav

    - Kept div tag for hero class since it is styling the photo only

    - Decided that the main content is the three sections (Search engine optimization, Online reputation management, Social media marketing). Replaced the div wrapping these sections with main

    - Replaced divs wrapping each individual section with the section tag (ie. Search engine optimization, Online reputation management, Social media marketing, Lead Generation, Brand Awareness, Cost Management).

    - Replaced div wrapping benefits section with aside tag

    - Replaced div wrapping h2 and p with footer tag

    - Added alt text to images - just in case images do not load

- CSS file repetitive/no longer working after switching divs with semantic elements
    - Replaced all the div elements in CSS file with the semantic elements that replaced it

    - Defined variables in CSS for colors that were used multiples times (only had to define two)

    - Saw that all the styling applied to the classes for the Search engine optimization, Online reputation management, Social media marketing sections had the same styling applied
        - Made the class name the same for those three sections and used that class to apply the same styling to all three sections without having to write out the same styling for each individual section 
            - Named the class 'miniSection'
        - Did the same thing for the benefitSection 
            - Removed the unnecessary lines of code in the CSS file

## Usage

![Alt Text](./assets/images/Website.png)

[Deployed Website](https://love4tau.github.io/Horiseon-HTML-CSS-Refactoring/)

## Credits

Juan Delgado: My tutor proofread my css and html files. Juan assisted with helping me gain a better understanding of where to apply the 'main' element. Juan also helped me realize that we can set the same class in the HTML file so we can apply the same styling to multiple sections. Ultimately, we were able to get rid of reptitive code in the CSS file.

https://www.w3schools.com/html/html5_semantic_elements.asp - referenced this website for semantic elements (Found aside element here)

https://coding-boot-camp.github.io/full-stack/github/professional-readme-guide - referenced this for the ReadME file
