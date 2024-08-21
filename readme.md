CSS:
1. Box Model: Content (fonts), padding, border, margin and outline 

3. overflow 
4. Colors (text, hash,RGB,rgba)

5. background & background-color
6. display inline - inline-block, block

7. flex
8. Positions 
9. Image width and height 
10. px and %

Media queries 
Opacity 

Block level: DIV, P, H1-H6, li
Inline: span, a, i, em, strong, b


==================================================================================================
1. Box Model
   > box-model: box-model mainly we can see in html elements. Box-model will have content/text,   padding, border and margin.
   > Around the content we have some space then it will known as padding.
   > Between padding and margin we have border
   > After the border we can have some space then it is called margin


2. What is Inline styles?
  > Styles which are written in the opening tag of html element then it is known as inline styles.
  > Disadvantage's: If we have same styles for multiple elements then its not recomanded because there would be a code redundancy(duplicate).
  > Alternative approach: we can use Internal Styles or External Styles (using class).
  Ex: <div style="padding: 10px;border: 1px solid rebeccapurple;margin: 10px;">Sample Text</div>

3. What is Internal Styles?
  > Internal styles we can use with in the same html document and we can use inside head tag using style element.
  > So inside the style element we can use selectors (class [.], id [#], psudeo [attributes])
  Ex: 
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Model</title>
    <style>
        .box-model{
            padding: 10px;
            border: 1px solid rebeccapurple;
            margin: 10px;
        }
    </style>
  </head>
  <body>
     <!-- Internal styles -->
     <div class="box-model">Sample Text_3 (INTERNAL STYLES)</div>
     <div class="box-model">Sample Text_4 (INTERNAL STYLES)</div>
  </body>

  4. What is External styles?
    > The styles which are defined other file with the externsion of .css or .scss then it is known as external styles
    > By using <link> element we can map the file.

  5. Difference between display none and visibiliy hidden
   > If we are using display none the element should not display/visible on webpage, It will remove the white space.
   > If we are using visibility hidden the element should be hidden or it shouldn't be visible/display on webpage but white space will remain same.

  6. anchore target use
   > If we give target="_black" then new tab will be opened. If we give target="_selft" it will open on same webpage/tab. By default if we not given target attribute then it will be open on same tab or webpage.

  7. overflow
   > we have 4 propertis (overflow-x, overflow-y,overflow-hidden and overflow-auto)
   > overflow-x : it will add horizental scrollbar, overflow-y: it will add vertical scrollbar.
   > overflow-hidden : If content is overflow then those will be hidden
   > overflow-auto : Automatically scrollbar will add if data is overflow either it may be horizental or vertical.

  8. Positions
   > positions is used to move the element into specific position, we can fixed the element at specific place and we can stick the element at specific place.
   > we have an different properties relative, absolute, fixed, sticky and static
   > Postition relative: It is used to move the element from any place to any place 
   > Position absolute: It is also same like as position relative but If we used combination of relative and absolute like as an ansyster(parent-child). parent as relative and child as absolute then if we can able to move absolute element with in the relative area.
   > Position fixed: It will fix the element at specific place.
   > Posistion sticky: It is used to stick the element along with the scroll.
   > Position static: Default behaviour of any element is position static.
   > Note: top, left, right and bottom these properties are works with positions only.

  9. Z-Index
  > Z-Index is used to arrange visibility stack order which one should visible on order.
  > Z-index property works with positions only.

  10. opacity
  > opacity its nothing but it will grayed out based on value.
  > value range from 0 - 1. If it is 0 element not display and 1 means it will display original color. In between 0-1 it will grayed out based on value.

  11. MinWidth and MaxWidth
  > MinWidth: It will take minimum width what you are specified and maximum it will take device width.
  > MaxWidth: It will take width upto specified maximum width. It won't take more than specified width.