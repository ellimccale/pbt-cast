# cast v2.0.5
cast is a theme skeleton built for the free forum software ProBoards. It's made up of basic adjustments to the default ProBoards theme, including a more neutral color scheme and multiple fixes to styles, layout templates, and markup. Its intended audience is intermediate to advanced users creating custom ProBoards themes. Those more familiar with CSS will find this theme easiest to customize through the stylesheet.

Built with the purpose of being redistributed as your own creation, you are free and encouraged to edit any part of this theme. You do not need to credit or reference me if you use this as a base for a premade or commission, but it would be cool to see what you build! That being said, a lot of personal time and effort were invested in tweaking and testing these files, and as such, my only request is that you don’t explicitly claim cast (as a base theme) as your own.

Be sure to review the [Readme PDF](cast-skin-readme.pdf) for additional information, the installation guide, and a bunch of super useful tutorials for various remodels (more coming soon). This also talks more about how to use the stylesheet and where to recolor the forum icons. Please reference this document before posting questions! It may already be answered.

If you’re less familiar with ProBoards themes or CSS/HTML, I would suggest reviewing these resources before getting started.

On ProBoards themes:
* http://adoxographyv2.boards.net/thread/1682/101-on-skin
* http://smangii.proboards.com/thread/38907/smangiis-theme-guide-proboards-v5

On CSS and HTML:
* http://htmldog.com/
* http://html.net/
* https://teamtreehouse.com/

## Use
1. You are **welcome** and **encouraged** to edit any part of this theme. It's meant to serve as a base for your own custom themes. You do not need to credit or reference me when submitting your creation as a premade.
2. You **are allowed** to remove any of my comments.
3. **Absolutely do not** claim **cast**, as a base theme, as your own. I've invested a lot of personal time and effort in these files.
4. **Absolutely do not** repost this theme without my permission. **Please notify me** if you see it posted outside of *Adoxography*, *ProBoards Support*, or GitHub.
5. You **are allowed** to pick and choose parts from cast. Feel free to download it to take what you need.

## Included
1. Predefined styles for the [Thread Descriptions](https://www.proboards.com/library/plugins/item/8) plugin
2. Predefined styles for sidebars
3. Predefined styles for more robust forum wrappers
4. A simple mixin for sticky navigation menus
5. [Smangii's ClearUBBC icons](http://smangii.proboards.com/thread/38879/clearubbc-icons-perfect-any-theme)
6. [Font Awesome](https://fortawesome.github.io/Font-Awesome/) icon glyphs

## Remodels
1. Removed box shadows and border radius mixins and CSS references
2. Reorganized the stylesheet with more descriptive comment headers and moved style blocks into more logical sections to make everything easier to search, read, and edit
3. Redefined a bunch of font family declarations with @default_forum_text_font_family to be consistent
4. Rebuilt info center to have less nested tables
5. Moved the footer content and bottom ads outside of the forum wrapper so they don't disrupt the inner spacing of the wrapper if it has a background color or image
6. Added styles to prevent the last .container div on the page from adding extra space to the forum wrapper if it has a background color or image
7. Replaced "like", "settings", "search", "locked", "bookmark", and "poll" icons with Font Awesome glyphs
8. Added styles and a script to darken the background overlay on modal windows
9. Made the padding on the user profile tables more consistent
10. Removed the extra right borders from the messages and conversations list templates
11. And tons more! See the [change log](CHANGELOG.md) for details

## Acknowledgements
Special thanks to [Smangii](http://smangii.proboards.com/user/1) for his [ClearUBBC icons](http://smangii.proboards.com/thread/38879/clearubbc-icons-perfect-any-theme), and [Trinity Blair](http://adoxographyv2.boards.net/user/1) for pointing out several of these fixes in her own Skeleton Theme.

## Installation
1. Download the [cast-skin.pbt](cast-skin.pbt) file and save it somewhere easily accessible, such as your Desktop or Downloads folder
2. Go to your forum’s Admin Panel
3. Click on **Themes > Theme Manager**
4. Click the “Create New/Import Theme” button
5. Click on “Import an Existing Theme”
6. Click the “Choose Theme File” button
7. Navigate to and select the cast-skin.pbt file
8. Once the theme has been imported, click the “Finished” button near the bottom right of the modal dialog window


**PROTIP:**
> If importing the .pbt file results in an error, you may need to try again. Sometimes the ProBoards theme importer fails despite multiple attempts. If the issue persists, try clearing your browser’s cookies and logging in again.
