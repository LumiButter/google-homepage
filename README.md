This is my first project! I dived into TOP eager to learn. I quickly got through the first sections until I arrived at the Code Camp tutorials. 

The tutorials were great, but it took a long time to complete. By the time I had, I had taken many breaks and completely forgot about the Command Line basics and GitHub basics.

Making the directory for this project was the first hurdle, and I think it's safe to say I'll be spending more time relearning these basics!

I'm excited to create my first real webpage. I have experience using Content Management Systems and Wix, but I never felt satisfied using them. I always felt there was something missing. I'm hoping this is the first step to finding those missing skills.

12/29/2020
    I started by creating a grid container to position the content. This should allow me to arrange the header, content, and footer appropriately.

    I then worked on the content area; placing the Google logo, creating the search bar, and the buttons.

    I thought it would be easy to create the shape of Google's search bar, but border-radius doesn't curve it correctly. I'm unsure how they styled it, so I'll look into it later. 

    Google's search bar doesn't change size when I resize the window, so I'm assuming it's a fixed height and width. I changed my search bar to be close to the same dimensions.

    The buttons were simple, just a fill with no border. There is a slight curve to the edges, so I applied a minimal border-radius. I'll make the colors match later when I Inspect the Google homepage.

    I thought the navbars would be easy, but they're more complex than I thought. It's interesting that I spent hours learning the coding basics from Code Camp, learning way more than this project requires, but still having trouble with the page. I have a new appreciation for webpages I think, the Google homepage looks simple but isn't when I try to build it.

    I don't know if my grid system will work anymore. I was originally going to create a three column grid:
    About, Store                            | BLANK | Gmail, Images, Menu, Sign In
    BLANK                                   |Content|BLANK
    Advertising, Business, How Search Works | BLANK | Privacy, Terms, Settings

    But spacing the individual buttons will be difficult, so it's better to make them each their own grid item and use the grid gap to space them. But, that would require a huge and uneven grid...While it's possible I don't think it's the most efficient way to handle it.

    I'll think more on this and return to it tomorrow.

    12/30/2020
    I started today by moving the header and footer out of the grid system. It will be easier creating fixed elements and placing the buttons inside them. 

    The first problem I noticed was my main content - the Google logo, search bar, and buttons - weren't aligned vertically. Adding the header as a fixed element meant it overlapped.

    The main content was still a grid item, so I tried to align it, but it didn't move. Makes sense, it's trying to align from within the grid...which is only one cell at this point. 

    I changed the container's position to fixed so I could position it correctly. Since the actual homepage isn't responsive I felt fine positioning it this way. It's still odd to have a one-item grid and two fixed elements, so maybe I'll redo the main content...

    I have the header, footer, and content all positioned correctly. But now I wonder if the original grid system would have worked. There's no reason every link needs it's own cell, I could create three columns and make each link it's own element and space them properly. I think two columns would work too, so I'm going to try that.

    Top-left | Top-right
    Content  | Content
    Bot-left | Bot-right

    The content will span both columns, meaning it should stay centered. I can push the other cells to the ends, creating a wide gap.

    The two grid system works well. Using justify-self to align the left and right cells to the ends creates close to perfect spacing. There are still problems of course.

    The top elements are fixed to the top like they should be, but the content appears right below them. I'm guessing I could fix this by making a huge row gap? There must be a better way to stick the bottom elements to the bottom...

    The bottom elements also aren't the correct color. The text I placed in them is highlighted gray, but the whole bottoms aren't gray. I'm going to try making the container element gray and make the content white.

    That didn't work. The cells are only as big as their content, so everything outside of them is the container. Now it's way too much gray. Is a fixed element at the bottom better then?

    I tried to align everything using a grid-row-gap, but as expected this didn't achieve what I wanted. It was trial and error to get a perfect gap, and it still won't stick the bottom element to the bottom. It also moves the main content too far down the page. 

    I'm going to take a break for today. Tomorrow I'll go through the Code Camp material to see if there's a way to arrange this grid how I want. If I can't find a good solution, my only other idea is manually positioning everything...I'd rather inspect the Google page instead.

    1/4/2021
    I've taken a few days off from this and am ready to figure out this problem. Before I go through the Code Camp material, I'm going to change the grid a bit. I'm going to create a container element for the footer and style that as needed.

    It looks like this works! It might be a little clunky and take too many divs, but it's positioned correctly. Now I'll make it a grid...

    The second grid works, and now the content is separated nicely. The text is too close to the top of the footer, so I'll need to reposition it a bit. I'll also need to change the style of the text and maybe create span elements to space the text correctly?

    The span elements ended up being perfect for spacing. Everything looks very similar, aside from the Settings link. It hugs the end of the container even with the padding and margins, though this might be because of the grid. 

    I'll work on creating the Sign In button next, then take a look at the Google homepage to make sure my formatting is correct. I'll need to find the right font, the font size, the correct colors, and then the source image for the menu button.

    1/19/2021
    Inspecting webpages is always interesting. The Google searchbar is a combination of div elements arranged in a flex display. Originally I tried to create all these styles in the input element, but I changed it to align with the actual Google page. 

    Copying this gave me a search bar that looks identical to Google's aside from the symbols. These are SVGs so I may be able to add them, but otherwise I'll refrain. The text field isn't aligned properly, I'll work on that.

    Adding the SVG didn't go as I planned. It broke free of the container and is way too big. More investigation needed...

    Fixed the issue. There was a second class on the original icon that formatted it. I'm curious why Google doesn't use meaningful names for their classes...

    After paying attention to these double class situations I have the box formatted correctly! The speech button doesn't show up, but I'm guessing there's an issue with the source image.

    I've finished setting my styles up to mimic Google. The last thing before I call the project finished is centering the search bar.

    Some observations: I built this page differently than Google did. Google uses a ton of div elements to align things how they want, and I'm unable to copy that without completely changing my design. I feel like it's not in the spirit of the project to change the work I've done to fit theirs. My spacing is off. My top links are closer to the top than they should be. My bottom links are closer to the edges than they should be. I can work to fix these things, but I can't rely on inspecting Google for them.

    With a few tweaks to margins, my page is almost identical to the original Google homepage.

FINAL THOUGHTS
    This project took four days of work spread across an entire month. It felt like a lot in the moment, but looking back I'm surprised it only took four days.

    I struggled more than I thought I would. I also developed an appreciation for the breadth of techniques in web development. The techniques I used to create this page are totally different than what Google used, and I suspect each TOP student has their own methods. For this reason, I don't feel like I did it the wrong way. There were issues with my method and surely ways to fix them.

    Since I struggled during this project, I want to tackle the optional project too. It's going to be harder and I know I'll struggle again, but I've shown myself that I need the experience.
