# ***Css Summary***

## Css Selectoers

### ***part1***

* [*] all elments
* Element => [p, div, h2]
* Element OtherElement => div p
* .class-name
* #id-name
* .parent.child          >>> element has a class child
* .class-one.class-two   >>>  elment has two class (one/two)
* .class-name div, .class-name p
* Element.class-name => p.class-name
* .parent > .child   => all  Child direct

### ***part2***

* Element + Other Element => [div + p]  >>> only element after
* Element ~ Other Elements => [p ~ div] >>> all elements after
* [Attribute]
* Element[Attribute]
* [Attribute=Value]
* Element[Attribute=Value]
* [Attribute~=Value] >>>  value containing a specified word. discrete
* [Attribute*=Value] >>> value contains a specified value.dis or con
* [Attribute|=Value] >>> value can be exactly the specified value ,or follow(-)
* [Attribute^=Value]  >>> starts with the specified value. dis or con
* [Attribute$=Value]  >>> ends with the specified value. dis or con

### ***part3***

#### ***Pseudo Classes***

* :first-child
* :last-child
* :first-of-type
* :last-of-type

___

* :not(Selectors)
* :nth-child(n)
* :nth-last-child(n)
* :nth-of-type(n)
* :nth-last-of-type(n)
* :only-child
* :only-of-type

___

* :root
* :checked
* :empty
* :disabled
* :required
* :focus
* ::selection
* ::placeholder
* ..etc

### ***Specificity Hierarchy***

If the style css is repeated for the same element, which one has priority for execution

1. !importand
2. Inline styles
3. ID
4. Class
5. Element and pseudo-element

## ***text***

* ***color***
  * name-color  ex >> ( <mark>color: red</mark> )
  * hex-code  ex >> ( <mark>#11111</mark>)
  * rgba    ex >> ( rgb(255, 99, 71 , 100%) )
  * hsla    ex >> ( rgb(255, 99, 71 , 100%) )

* ***text-align***
  * center
  * left
  * right
  * justify

* ***text-align-last***  
property for the last line
  * center
  * left
  * right
  * justify

* ***text-direction***
  * rtl  [right-to-left]
  * ltr  [left-to-right]

* ***writing-mode***
  * horizontal-tb
  * vertical-rl

* ***vertical-align***  
property sets the vertical alignment of text with element(img etc...)
  * top
  * middle
  * sub
  * super

* ***text-decoration***  
this is shorthand prope*
  * text-decoration-line
    * underline
    * overline
    * line-through
    * none
  * text-decoration-color
    * name color
  * text-decoration-style
    * solid
    * dotted
    * dashed
  * text-decoration-thickness

```css
text-decoration: line color style thickness;
```

* ***text-transform***
  * capitalize
  * lowercase
  * uppercase

* ***text-indent***  
Specifies the indentation of the first line in a text
  * px
* ***letter-spacing***  
the space between characters in a text
  * px
* ***line-height***  
the space between lines
  * px
* ***word-spaceing***  
the space between characters in a word
  * px
* ***white-space***  
how to handle white-space inside an element
  * normal
  * nowrap
  * break-all
  * break-word

### ***text wrap***

* ***white-space***
  * nowrap
* ***text-overflow***
  * clip
  * ellipsis
* ***word-wrap***
  * break-word
* ***break-word***
  * keep-all
  * break-all

___

___

## ***Background***

### background

this is shorthand property

```css
background: color image repeat attachment position ;
```

* ***background-color***
  * color
* ***background-image***
  * url('relative url / absoluteurl ')
* ***background-repeat***
  * repeat
  * no-repeat
  * repeat-x
  * repeat-y
* ***background-attachment***
  * fixed
  * scroll
* ***background-position***
  * ?px ?px
  * ?%  ?%
  * left / right / top / middle
  * left top / bottom right / top right ..etc
* ***background-size***
  * cover
  * contain
  * ?px ?px
  * ?%  ?%
* ***background-origin***  
where the background image(s) is/are positioned
  * border-box
  * padding-box
  * content-box
* ***background-clip***  
Specifies the painting area of the background
  * border-box
  * padding-box
  * content-box

### ***gradient***

* linear-gradient  

```css
background-image: linear-gradient(to direction , color1, color2,..);
background-image: linear-gradient(angel , color1, color2 ..);
/* repeating gradient */
background-image: repeating-linear-gradient(to direction , color1, color2 ,..);
background-image: repeating-linear-gradient(angel , color1, color2 ..);
```

* radial-gradient

```css
background-image: radial-gradient(circle, red, yellow, green);
/* repeating gradient*/
background-image: repeating-radial-gradient(circle, red, yellow, green);
```

* conic-gradient

```css
background-image: conic-gradient(red, yellow, green, blue, black);
/* repeating gradient*/
background-image: repeating-linear-gradient(red, yellow, green, blue, black);
```

## ***Display***

### ***Block***

* Take Full Width screen If No have Width
* Add Line Break
* Respect Padding, Margin, Width, Height

### ***Inlnie-block***

* Allow Elements Before And After It in The Same Line
* Respect Padding, Margin, Width, Height

### ***Inline***

* Do Not Repsepct Width, Height
* Respect Padding And Margin >> only [ right + Left ]
* Do Not Add Line Break
* Allow Elements Before And After It in The Same Line

### ***Properites***

* ***Display***  
specifies how the element display
  * block
  * inline-block
  * inline
  * none >> The element is  removed from page
  * flex
  * grid
  * ...etc
  
* ***visibility***  
Specifies the element is visible or hidden
  * visible
  * hidden

## ***Border***

* ***border-style***  
how the border is display
  * solid
  * dotted
  * dashed
  * ..etc
* ***border-color***
* ***border-width***

### ***Border Shorthand***

```css
border: width style color;
/* example */
border: 10px solid red;
```

* ***border-raduis***  

* ***border-spacing***  
used in table to determine space between border cells in border table

* ***resize***  
property used with textarea input to resize input with user or no
  * auto
  * none
  * horizontal
  * vertical
  * both

## ***Shadow***

### ***text-shadow***

```css
text-shadow: [horizontal] [vertical] [blur] [color];
/* example */
text-shadow: 2px 2px 4px red;
```

### ***box-shadow***

```css
/* shadow out box */
box-shadow: [horizontal value] [vertical vlaue] [ blur ] [spread] [color];
/* shadow in box */
box-shadow: [horizontal value] [vertical vlaue] [ blur ] [spread] [color] [inset];
/* example */
box-shadow: 2px 2px 4px 3px red;
box-shadow: 2px 2px 4px 3px red inset;
```

### ***box-reflect***

A reflection of the image

* ***box-reflect***
  * right
  * left
  * below

## ***Units***

***there are two type of length units absolute and relative***

* Absoloute Lengths  
are fixed and a length expressed in any of these will appear as exactly that size.
* Relative Lengths  
Relative length units scale better between different rendering mediums.

### Absolute lengths

| Unit | Description |
|------|-------------|
| cm | centimeters |
| mm | millimeters |
| in | inches(1in = 96px = 2.54cm) |
| px | pixels  |
| pt | pionts  |
| pc | picas (1pc = 12 pt) |

* Pixels (px) are relative to the viewing device. For low-dpi devices,

### Relative lengths

| Unit | Description |
|------|-------------|
| em | default font size for root or current size |
| ex | half of current size |
| ch | ????????????? |
| rem | Relative to font-size of the root element |
| vw | Relative to 1% of width of the viewport |
| vh | Relative to 1% of height of the viewport |
| vmin | Relative to 1% of viewport's* smaller dimension |
| vmax | Relative to 1% of viewport's* larger dimension |
| % | Relative to the parent element |

## ***Font***

list are the best web safe fonts for HTML and CSS:

1. Arial (sans-serif)
2. Verdana (sans-serif)
3. Tahoma (sans-serif)
4. Trebuchet MS (sans-serif)
5. Times New Roman (serif)
6. Georgia (serif)
7. Garamond (serif)
8. Courier New (monospace)
9. Brush Script MT (cursive.

super-family  >>> the Lucida superfamily contains the following fonts:

1. Lucida Sans
1. Lucida Serif
1. Lucida Typewriter Sans,
1. Lucida Typewriter Serif
1. Lucida Math.  

### ***properties***

* ***font-family***
* ***font-style***
  * normal
  * italic
  * oblique
* ***font-weight***
  * normal
  * bold
  * bolder
  * (100 200 300 .... 900)
* ***font-varient***
  * normal
  * small-caps
* ***font-size***

### ***font-shorhand***

```css
font: [style] [varient] [weight] [size/line-height] [family];
/* example */
font: italic bold 20px blue ;
```

font (size / family) values are required for font shorhand

## ***Position***

### ***position***

* static >>> is default value
* relative
* Absolute
* sticky
* fixed
  
## ***transition***

### ***transition-shorthand***

property is the shorthand for

* transition-duration
* transition-delay
* transition-property
* transition-timing-function

```css
transition: [duration] [delay] [property] [time-function]; 
```

### ***transition-delay***

Specifies a delay (in seconds) for the transition effect

* ***transition-delay***
  * seconds (1s)
  * milliseconds (1000ms = 1s)

### ***transition-duration***

how many seconds or milliseconds a transition effect takes to complete

* ***transition-duration***
  * seconds (1s)
  * milliseconds (1000ms = 1s)

### ***transition-property***  

Specifies the CSS property the transition effected by duration and delay

* ***transition-property***  
  * name-property

### ***transition-timing-function***

* ***transition-timing-function***  
Specifies the speed curve of the transition effect
  * ease >>> default value
  * linear
  * ease-in
  * ease-out
  * ease-in-out

## ***flexbox***

### ***flex property for parent***

___

* ***display***
  * flex
  * inline-flex
* ***flex-direction***
  * row >> (default value)
  * row-reverse
  * column
  * column-reverse  

![descripe direction](https://cdn.hashnode.com/res/hashnode/image/upload/v1592610331847/JboMfMpab.jpeg?auto=compress,format&format=webp)

* ***flex-wrap***
  * wrap  >> (default value)
  * nowrap
  * wrap-reverse  

![descripe wrap](https://cdn.hashnode.com/res/hashnode/image/upload/v1592610466031/URTwerTEU.png?auto=compress,format&format=webp)

* ***flex-flow***
  * [flex-direction]+[flex-wrap]

```css
flex-flow: column wrap-reverse ;
```

![descripe flex-flow](https://cdn.hashnode.com/res/hashnode/image/upload/v1592610517892/2LRbRRnu_.png?auto=compress,format&format=webp)

## ***justify-content***
  
***property is used to align the flex items:***  
**if flex-direction => row  >>> to align horizontal**  
**if flex-direction => column  >>> to align vertical**

* ***justify-content***  
  * flex-start >> (default value)
  * flex-end
  * center
  * space-between
  * space-around
  * space-evenly  

### ***justify-content [flex-direcrion: row]***

![descripe justify](https://miro.medium.com/v2/resize:fit:640/format:webp/1*iigDGiNFBOUVJQ_07C1B2g.png)

### ***justify-content [flex-direcrion: column]***

![descripe justify](https://dirask.com/static/bucket/1624478985957-ZBA8Ee1Q5K--image.png)

## ***align-items***  

***property is used to align the flex items:***  
**if flex-direction => row  >>> to align vertical**  
**if flex-direction => column  >>> to align horizontal**  

* ***align-items***  
  * stretch >> (default value)
  * flex-start
  * flex-end
  * center
  * space-between
  * space-around
  * space-evenly  
  * beseline

### ***align-items [flex-direcrion: row]***

![descripe items](https://miro.medium.com/v2/resize:fit:640/format:webp/1*UN38NMI1knNTwX6HbV0oYA.png)

### ***align-items [flex-direcrion: column]***

![descripe items](https://samanthaming.gumlet.io/flexbox30/17-align-items-column.jpg.gz)

## ***align-content***  

***without flex-wrap =>> is not worked***  

**property is used to align the flex all items :**  
**if flex-direction => row  >>> to align vertical**  
**if flex-direction => column  >>> to align horizontal**  

* ***align-content***  
  * stretch >> (default value)
  * flex-start
  * flex-end
  * center
  * space-between
  * space-around
  * space-evenly

![descripe content](https://images.squarespace-cdn.com/content/v1/63906395ddb295734cb00d3c/b1f75c1b-721e-49f5-93eb-aa0751be1379/in-depth-12.png)

### ***flex property for child***

___

* ***felx-grow***  

default value = 0
![descripeGrow](https://samanthaming.gumlet.io/flexbox30/21-flex-grow.jpg.gz?format=auto&width=500)
![descripeGrow](https://res.cloudinary.com/practicaldev/image/fetch/s--DAv1Nq97--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/7vs74vcb2fwuukj9fid6.png)

* ***flex-shrink***  

default value = 1
![descripeshrink](https://cdn.hashnode.com/res/hashnode/image/upload/v1592610914528/NnrkheWqy.jpeg?auto=compress,format&format=webp)
![descripeshrink](https://res.cloudinary.com/practicaldev/image/fetch/s--TnNT8w9M--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/h31qniw74ffrp4lkwitz.png)

* ***order***

default value = 0

![descripeOrder](https://samanthaming.gumlet.io/flexbox30/20-order.jpg.gz?format=auto&width=500)

* ***flex-basis***  
specifies the initial length of a flex item.

default value = 0
![descripeGrow](https://samanthaming.gumlet.io/flexbox30/25-flex-basis.jpg.gz?format=auto&width=500)

* ***align-self***  
  * flex-start
  * flex-end
  * center
  * stertch
  * baseline
  * auto

![describeSelf](https://res.cloudinary.com/practicaldev/image/fetch/s--F9xzTLNM--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zhbmzijiqvzbzlwjhmt0.png)

![describeSelf](https://cdn.hashnode.com/res/hashnode/image/upload/v1592611004580/EpQVlMJm8.png?auto=compress,format&format=webp)

* ***flex***  
is the shorthand for flex-grow , flex-shrink and flex-basis

```css
flex: [flex-grow] [flex-shrink] [flex-basis] ;
```

## ***grid***

### ***grid property for parent***

___

* ***display***
  * grid
  * inline-grid
* ***grid-template-columns***  
[Number Of Columns In] => [Px, %, Auto, Fraction, Repeat(), Mix]  
* ***grid-template-rows***  
[Number Of Columns In] => [Px, %, Auto, Fraction, Repeat(), Mix]  

![descripeColumnsRows](https://files.codingninjas.in/article_images/css-grid-0-1635273728.webp)
![descripeColumnsRows](https://pbs.twimg.com/media/FQ34hYPUUAQYXpi?format=jpg&name=4096x4096)

* ***row-gap***
* ***column-gap***
* ***gap***

![descripegap](https://miro.medium.com/v2/resize:fit:1202/1*wJnQG4MuYMLSqkZS93TCvw.png)

* ***grid-tempalet-areas***
* ***justify-content***
* ***align-content***

#### ***grid-temlate***

is the shorthand for grid-template-columns adn grid-template-rows

```css
grid-template: [rows]/[columns];
/* example */
grid-template: repeat(3,1fr) / repeat(5,1fr); ;
```

### ***grid property for child***

___

* ***grid-colunn-start***
* ***grid-colunn-end***
* ***grid-colunn***  
the property is shorthand for:
  * grid-column-start
  * grid-column-end

```css
grid-column: [start] / [end];
grid-column: [start] / span?? ;
/* example */
grid-column: 1 / 4 ;  /* first three columns */
grid-column: 0 / span3 ;  /* first three columns */
```

* ***grid-row-start***
* ***grid-row-end***
* ***grid-row***  
the property is shorthand for :
  * grid-row-start
  * grid-row-end

```css
grid-rows: [start] / [end];
grid-rows: [start] / span?? ;
/* example */
grid-rows: 1 / 4 ;  /* first three rows */
grid-rows: 0 / span3 ;  /* first three rows *rows */
```

* ***grid-area***  
the property is shorthand for
  * grid-column-start
  * grid-column-end
  * grid-row-start
  * grid-row-end

```css
grid-area: [row-start] / [column-start] [row-end] / [column-end];
```

## ***mouse***

___

### ***cursor***

property sets the mouse cursor, if any, to show when the mouse pointer is over an element.

* ***cursor***
  * auto
  * pionter
  * gap
  * zoom-in
  * zoom-out
  * help
  * wait
  * ...etc
  
### ***pionter-event***

property defines whether or not an element reacts to pointer events.

* ***pionter-event***
  * none
  * auto
  * initial
  * inherit

### ***caret-color***

property sets the color of the insertion caret

* ***caret-color***
  * color
  
### ***:selection***

when the selected text shows color and background distinct other than backgound blue and color black

![show](https://www.myphone.pl/wp-content/uploads/2018/02/android7-copy-paste.gif)

* ***selection***
  * color
  * background

```css
*::selection {
  color: red;
  background: yellow;
}
```

## ***Transform***

### ***Transform 2D***

___

#### ***TRANSLATE***

method moves an element from its current position

* ***translate***
  * translateX()
  * translateY()
  * translate( X , y ) >>>  [shorthand]

```css
transform: translate( 50px , 50px );
```

#### ***ROTATE***

method rotates an element clockwise or counter-clockwise

* ***rotate*** with **deg**
  * deg => degree
  * rad => radians
  * garad => gradians
  * turn

```css
transform: rotate( 45deg );   /* clockwise  */
transform: rotate( -45deg );  /* counter-clockwise */
```

#### ***SCALE***

* ***scale***
  * scaleX()
  * scaleY()
  * scale()

```css
transform: scale( 2 , 2 );
transform: scale( 2 );   /* value for X and Y */
```

#### ***SKEW***

* ***skew*** with **deg** / **rad** / **grad**
  * skewX()
  * skewy()
  * skew()

```css
transform: skew( 45deg , 10deg );
transform: skew( -45deg , -10deg );
```

#### ***MATRIX***

the property is the shorthand for

1. scaleX()
2. skewX()
3. skewY()
4. scaleY()
5. translateX()
6. translateY()

write with order

```css
transform: matrix(1, -0.3, 0, 1, 0, 0)
```

#### ***origin***

property allows you to change the shape center of element  
take two value prcentage or direction

* ***origin***
  * 50% 50% >>> defalut value
  * center center >>> defalut value
  * top right
  * bottom right

### ***Transform 3D***

___

#### ***rotate 3D***

* ***rotate***
  * rotate3d >>> (X-axis , Y-axis , Z-axis ,angle)
  * roteateX()  
rotate an element around its X-axis
  * roteateY()  
rotate an element around its Y-axis
  * roteateZ()  
rotate an element around its Z-axis

```css
transform: rotate3d(1, 1, 1, 45deg);
```

#### ***translate 3D***

* ***translate***
  * translate3d(X-axis ,Y-axis ,Z-axis )
  * translateZ()

```css
transform: translate3d(42px, -62px, -135px);
```

#### ***prespective***

property determines the distance between page and the user

* ***prespective***
  * none
  * 20px for example
  * initial
  * inherit

#### ***prespective-origin***

* ***prespective-origin***
  * X-position Yposition
  * 50% 50%
  * direction >>> (left / top / right / bottom)
  * top left
  * bottom right

#### ***transform-style***

* ***transform-style***
  * flat >> default value
  * preserve-3d

#### ***backface-visibility***

* ***backface-visibility***
  * hidden  >> (default value)
  * visible

## ***Animation-***

### ***@keyframmes***

controls the intermediate steps in a CSS animation sequence by defining styles for keyframes (or waypoints) along the animation sequence

```css
@keyframes animation-name {
  from { property: value;}
  to { property: value; }
}
/* or */
@keyframes animation-name {
  0% { property: value;}
  25% { property: value;}
  50% { property: value;}
  100% { property: value;}
}
```

### ***animation-duration***

property defines how long an animation should take to complete.

* ***animation-duration***
  * 1s
  * 1000ms

### ***animation-delay***

property specifies a delay for the start of an animation.

* ***animation-delay***
  * 1s
  * 1000ms

### ***animation-iteration-count***

specifies the number of times an animation should run.

* ***animation-iteration-count***
  * number
  * infinite

### ***animation-direction***

property sets whether an animation should play forward, backward, or alternate back and forth between

* ***animation-direction***
  * normal
  * reverse
  * alternate
  * alternaet-reverse

### ***animation-fill-mode***

property sets how a CSS animation applies styles to its target before and after its execution.

* ***animation-fill-mode***
  * forwards
  * backwords
  * both

### ***animation-play-state***

property sets whether an animation is running or paused.

* ***animation324***
  * paused
  * running

### ***animation-timing-function***

property sets how an animation progresses through the duration of each cycle.

* ***animation-timing-function***
  * ease
  * linear
  * esae-in
  * ease-in-out

### ***animation***

property is  the shorthand for

* animation-name
* animation-duration
* animation-delay
* animation-direction
* animation-fill-mode
* animation-iteration-count
* animation-play-statث
* animation-timing-function
* animation-timeline

```css
animation: 3s ease-in 1s 2 reverse both paused animation-name;
```

## ***Global Values***

### ***inherit***

* ***inherit***
  * take the computed value of the property from its parent element.

```css
.parent{
  color: orange;
}
.parent > div {
  color: inherit; /*color = orange  */
} 
```

### ***initial***

* ***initial***
  * the initial (or default) value of a property to an element. It can be applied to any CSS property

### ***unset***

resets a property to its inherited value if the property naturally inherits from its parent, and if not inherit value will be reset to initial value
  
* ***if inherit property***  
  the property will be inherit valuie

* ***if not inherit property***  
  the property will be initial value

### ***all***

* ***all***

property resets all of an element's properties except ***unicode-bidi***, ***direction***, and ***CSS variables***

* It can set properties to their :
  * initial value
  * inherit value
  * revert (user agent property)

### ***revert***

back to the property speicifie for user agent

## ***Links pesudu classess***

* ***a:link***  
  a normal, unvisited link
* ***a:visited***  
  a link the user has visited    >> visted link
* ***a:hover***  
  a link when the user mouses over it   >> hover mouse a link
* ***a:active***  
  a link the moment it is clicked      >>  when active link only

***A:HOVER*** must come after ***A:LINK*** and a:visited  
***A:ACTIVE*** must come after ***A:HOVER***

<!-- * :target  
Selects the current active #news element (clicked on a URL containing that anchor name) -->

<!-- attr for html edit content
contenteditable="true"
 -->

<!-- ## ***inputs pesudu classess***

* ***input date *** -->
