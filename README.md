[flowers](http://tlwr.github.io/flowers)
==
The css framework for responsive page layouts.

Pages
==

Flowers defines a page as an element taking up a proportion of the whole viewport.
You can define a page by applying the class `page`.

You define how large the minimum height of a page is by adding a class.  
For instance a page taking up half the height of the viewport has the class `half`.

If you want to force a page to be a certain height you add the class `force`.

An example of a 4 page website would look something like this:
```
<body>
  <section class="page half">The first page</section>
  <section class="page half">The second page</section>
  <section class="page full">The third page</section>
  <section class="page double force">The fourth page.</section>
</body>
```
In this example, the last page does not change height to fit the elements inside.

| Proportion of Page | Class     |
| ------------------ | --------- |
| 20%                | `fifth`   |
| 25%                | `quarter` |
| 33%                | `third`   |
| 50%                | `half`    |
| 100%               | `full`    |
| 200%               | `double`  |
| 300%               | `triple`  |
| 500%               | `five`    |
| 1000%              | `ten`     |

Alignment
==

Flowers uses flexbox to align things, this allows for easy vertical alignment of child elements.

Basics
--

To align things, the container should have the class `align`.

If the container should stay inline, it should have the class `align-inline`.

If the children should be in a row, the container should have the class `row`.  
If you want a reversed row, use the class `row-rev`.

If the children should be in a column, the container should have the class `col`.  
Likewise, if you want a reversed column, use the class `col-rev`.

If you want to keep the children from wrapping, on the container use the class `nowrap`, otherwise, use `wrap`.

Horizontal Alignment
--

Apply these classes to the parent. If you are using `row-rev`, these effects will be reversed.

| Effect                              | Class            |
| ----------------------------------- | ---------------- |
| At the start                        | `h-item-start`   |
| At the end                          | `h-item-end`     |
| In the center                       | `h-item-center`  |
| Space around (before and after)     | `h-item-space-a` |
| Space between (in between elements) | `h-item-space-b` |

Vertical Item Alignment
--

Apply these classes to the parent.  
These classes will change the way items are aligned on the current line, not the whole content box.

| Effect                                      | Class             |
| ------------------------------------------- | ----------------- |
| At the start                                | `v-item-start`    |
| At the end                                  | `v-item-end`      |
| In the center                               | `v-item-center`   |
| Stretch the content to fit the height       | `v-item-stretch`  |
| Align items with each others' text baseline | `v-item-baseline` |

Vertical Content Alignment
--

Apply these classes to the parent.
These classes will change the way items are aligned across the whole content box.

| Effect                              | Class               |
| ----------------------------------- | ------------------- |
| At the start                        | `v-content-start`   |
| At the end                          | `v-content-end`     |
| In the center                       | `v-content-center`  |
| Space around (before and after)     | `v-content-space-a` |
| Space between (in between elements) | `v-content-space-b` |
| Stretch all the elements to fit     | `v-content-stretch` |

Element Sizing
--

If you have wrapping on, you can apply these to the children to force sizing.

In this example, the last page does not change height to fit the elements inside.

| Size | Class     |
| ---- | --------- |
| 20%  | `fifth`   |
| 25%  | `quarter` |
| 33%  | `third`   |
| 50%  | `half`    |
| 100% | `full`    |

Lists
--

To a `<ul>` or an `<ol>` you can add the class `blank` to remove the list style, and the class `none` to remove the indentation.

Text
--

###Font Variations
`italic` italicises the text  
`oblique` applies an oblique effect  
`smallcaps` makes the text small caps  
`lowercase` forces lowercase  
`uppcase` forces uppercase
`capitalize` forces capitalisation  
`capitalise` is an alias for capitalize  
`ellipsis` will, upon text break, make an ellipsis instead
`text-line-none` forces no decoration  
`text-line-over` forces an overline  
`text-line-under` forces and underline  
`text-line-through` forces a strikethrough
`text-center` makes the text centered  
`text-left` makes the text left aligned  
`text-right` makes the text right aligned

###Font weights

| Weight | Class      |
| ------ | ---------- |
| 100    | `lightest` |
| 200    | `lighter`  |
| 300    | `light`    |
| 400    | `book`     |
| 500    | `medium`   |
| 600    | `mediumer` |
| 700    | `bold`     |
| 800    | `bolder`   |
| 900    | `boldest`  |

