## Push and pull column

A special [push and pull class](http://foundation.zurb.com/sites/docs/grid.html#source-ordering) allows us to change the order of the columns.


```
<div class='row'>
  <div class='small-9 columns'>Content</div>
  <div class='small-3 columns'>Sidebar</div>
</div>

<div class='row'>
  <div class='small-9 small-push-3 columns'>Content</div>
  <div class='small-3 small-pull-9 columns'>Sidebar</div>
</div>
```

HTML defines the order of the content. The order shows how important the content is. More important content are placed before other content.

When we float the columns from left to right. It follows the order of the column divs.

For instance, if we want to swap the side bar from right to left, we can either change the HTML or we can change the CSS class by using this foundation class. Both code result in the same output visually. So what is the difference?

The difference is that the foundation class solution doesn't change the order of the HTML element. We keep the same definition that content is more important than the side bar. But visually, we have our choice to define whether the side bar goes to the left or right side visually.
