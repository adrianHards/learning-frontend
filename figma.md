# Figma-tips-for-UI-design

## Learn the most common shortcuts

Rectangle tool   `R` 

Move tool        `V`

Type tool        `T` 

Ellipse tool     `O`

Frame tool       `F`

Zoom in          `⌘ +` 

Zoom out         `⌘ -`

Zoom 100%        `⌘ + 0`

Toggle grid      `⌃ + G`

Group Selection  `⌘ + G`

Big Nudge        `⇧ + direction`

Duplicate        `Option + drag`

Show/hide tool panel  `⌘ + .`



## Shortcut resources
- [Figma shortcuts](https://shortcuts.design/toolspage-figma.html)


## Learn about layout and the 8pt grid system

Designers love grids, they help create rhythm and structure to your layouts. 

A good place to start is with the 8pt grid system. The 8pt grid is a spacing system which uses multiples of 8. 8, 16, 32, 64, 128 and so on. 

Using a system for sizing and spacing elements creates constraints, prevents the use of arbitrary values and improves the consistency in your designs. 

How does this work in Figma?

### Setting up Layout Grids

First click the hamburger icon in the top left corner of the Figma app. Scroll down to _preferences_ > _nudge amount_ and make sure the value for _small nudge_ is set to 1 and the value for _big nudge_ is set to 8.

Now create a new frame by pressing `f` on your keyboard, and selecting _Desktop_ > _MacBook Pro_ from the properties panel on the right side of the app.

With the frame selected, you will see the Layout Grid option, greyed out in the same properties panel on the right. Clicking on the `+` icon or the name will create a new 8pt grid.

Now when you draw out shapes they will snap to the grid.

### Layering grids to create columns and rows

With the frame selected click the `+` button next to Layout grid once more to create another grid on top. This time hit the icon to the left of ‘Grid (8px)’ and switch grid to columns. 

To keep things simple set _Count_ to 4, _Margin_ to 64 and _Gutter_ to 32. Notice these values all work with the 8pt grid.

Your columns should be nicely aligned with your 8pt grid below.

### Nesting your frames to create interesting layouts

Unlike with other software, which use fixed artboards, in Figma you can nest frames within frames to create interesting layouts. This is useful designing components with different layout or grids.

### Grid and layout resources
- [Intro to The 8-Point Grid System](https://builttoadapt.io/intro-to-the-8-point-grid-system-d2573cde8632)
- [Frames within frames](https://www.figma.com/blog/grid-systems-for-screen-design/#frames-within-frames)

## Create a type system

Oliver Reichenstein once said; “Web design is 95% typography, so it’s only logical to say that a web designer should get good training in the main discipline of shaping written information.“

I tend start with a free typeface designed for UI, such as Inter or San Fransisco UI, which are both ideal for prototyping and have a range of weights.

Approach type exactly how you would in code. Before you start designing, first create a scale of type sizes and line heights, starting with the body text, as this is what there will be most of. Sizes don’t have to be spot on at this stage, you can always change them later.

For example if my body copy is 20px, I might multiple the text size by 1.6 to get a line-height of 32px. You can actually do this maths directly in the _Line height_ field: `20*1.6` + `Enter`. This is a good line-height for body copy.

Next tackle the scale for your headings. I tend to set headings in a bolder weight to provide enough contrast between the regular weight of the body text. A line height of 1.2 is usually a good bet for larger heading sizes.

Creating a system like this creates constraints in your work and helps to keep your designs feeling consistent. 


### Type system resources
- [Typography systems in Figma](https://www.figma.com/best-practices/typography-systems-in-figma/)
- [Web Design is 95% Typography](https://ia.net/topics/the-web-is-all-about-typography-period)


## Use the dimensions palette to size things

You can do maths in the dimensions palette too. This is ideal for sizing elements on your page to your 8pt or 4pt system.


## Understand colour and color styles

Create a primary palette including brand colour and tints.

Create greyscale palettes - one for surface colours (light greys or very dark greys for a dark theme) and one for text (dark greys or very light/white for dark themes). 

If the darkest grey you use is say 90% black and your lightest grey is 5% black, then avoid middle greys (40%, 50%, 60%). These are an accessibility nightmare. 

Make sure you use a contrast checker plugin like Able or Stark to check the contrast between your text and the background layer are accessible. 

Create a secondary palette for UI feedback colours (success, error, warning, info alerts).

If you’re not confident with colour, keep colours to a minimum 


### Colour resources
- [Color in Design Systems](https://medium.com/eightshapes-llc/color-in-design-systems-a1c80f65fa3)
- [Color in UI design a practical framework](https://medium.com/@erikdkennedy/color-in-ui-design-a-practical-framework-e18cacd97f9e)
- [A guide to color accessibility in product design](https://medium.com/inside-design/a-guide-to-color-accessibility-in-product-design-516e734c160c)

## Use Auto Layout

Auto layout is a powerful feature that can help you improve your workflow for anything from simple UI elements like buttons to complex responsive UI patterns list navigation and cards.

Figma has a great demo of how this work. I recommend you have a look and play around. It’s the only way to learn! 😎

### Auto layout resources
- [Create dynamic designs with Auto Layout](https://help.figma.com/hc/en-us/articles/360040451373-Create-dynamic-designs-with-Auto-Layout)
- [Quick tips for Auto Layout in Figma](https://uxdesign.cc/quick-tips-for-auto-layout-in-figma-411c639a51b0)


## Use plugins

Figma has a great developer community who have built some awesome tools that you can use for free. 

So before you start designing flows you might want to check out the Autoflow plugin, which makes it easy to draw flows automatically. Or uses the Unsplash plugin to insert licence free images straight into your designs.

Another great plugin is 

Plugins can be installed from the project overview in the top left sidebar. Use them, they will save you time and make you more efficient.


### Plugin resources
- [The 15 best Figma plugins for designers](https://uxdesign.cc/the-15-best-figma-plugins-for-designers-so-far-84332ab1a61)
- [Design for everyone with these accessibility-focused plugins](https://www.figma.com/blog/design-for-everyone-with-these-accessibility-focused-plugins/)
- [Behind the Plugins: Matt DesLauriers, Generative Artist & Creative Coder](https://www.figma.com/blog/behind-the-plugins-matt-deslauriers/)


## Join the Figma community

[On Spectrum](https://spectrum.chat/figma/)


