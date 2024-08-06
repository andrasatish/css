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


=========================================================
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