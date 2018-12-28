## Block grid

[Block grid](http://foundation.zurb.com/sites/docs/grid.html#block-grids) is a very powerful grid in Foundation.

> Block grids are a shorthand way to create equally-sized columns. Add a class of the format .`[size]-up-[n]` to change the number of columns within the row. By default, the max number of columns you can use with block grid are 8. Adding the `.column-block` class to columns will apply a bottom margin equal to the width of gutters.

It’s very useful for showing a collection of items into a grid.

```
<ul class="row small-up-2 medium-up-3 large-up-4">
  <li class="column column-block"><img src="http://placehold.it/300x200" alt="placeholder" /></li>
  ...
  <li class="column column-block"><img src="http://placehold.it/300x200" alt="placeholder" /></li>
</ul>
```

