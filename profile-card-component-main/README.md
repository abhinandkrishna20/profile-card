# Frontend Mentor - Profile card component

hey guys these is one of the challenges i get interesting in frontend metor since it it seems easy but
challenging!
the main goal of these design is not designing the card ,it is setting the two SVG backgrounds at the
back of the card so how could we do it since we cnat set it like othe svg backgrounds?
->i completed these design using CSS property :before and :after ,so the logic is
1]to have a container with SVG backgrounds that holds some content in it so i put the container
position #relative so that i can position my svg backgrounds absolute to the container.
2]don't forget to put overflow hidden and min-height 100vh for container and also z-index -1(to drag background at the back of content)

3]so our pseudoelments after and before has commmon properties both are
..width and height 100vw and 100vh
...z-index -1
...and position #absolute
4]since for the top svg background i use ::before and for bottom ::after according to there position
5].container:before i set position from top:0 and left:0;[center screen/default position ]
6].container:after i set position from top:100% and left 100%; [out of screen]
7]i use translate property for both of them transform:translate(-50%,-50%);
8]the translate property will drag each of the 50% from right and 50% from bottom
9] i use background: url('/images/bg-pattern-top.svg') no-repeat bottom right; /_to expand to bottom and right_/ for :before
and background: url('./images/bg-pattern-bottom.svg') no-repeat top left; /_to expand to top and left_/ for :after
![Design preview for the Profile card component coding challenge](./design/desktop-preview.jpg)

## Welcome! 👋

Thanks for checking out this front-end coding challenge.

[Frontend Mentor](https://www.frontendmentor.io) challenges help you improve your coding skills by building realistic projects.

**To do this challenge, you need a basic understanding of HTML and CSS.**

## The challenge

Your challenge is to build out this profile card component and get it looking as close to the design as possible.

You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

Want some support on the challenge? [Join our Slack community](https://www.frontendmentor.io/slack) and ask questions in the **#help** channel.

## Where to find everything

Your task is to build out the project to the designs inside the `/design` folder. You will find both a mobile and a desktop version of the design.

The designs are in JPG static format. Using JPGs will mean that you'll need to use your best judgment for styles such as `font-size`, `padding` and `margin`.

If you would like the design files (we provide Sketch & Figma versions) to inspect the design in more detail, you can [subscribe as a PRO member](https://www.frontendmentor.io/pro).

You will find all the required assets in the `/images` folder. The assets are already optimized.

There is also a `style-guide.md` file containing the information you'll need, such as color palette and fonts.
