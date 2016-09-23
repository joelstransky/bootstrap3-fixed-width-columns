# bootstrap3-fixed-width-columns
Generate classes for fixed width columns.

This only applies to columns who are children of a `.container`. Fixed width's would have to be re-calculated at runtime if used within `.container-fixed`

[demo](http://codepen.io/JoelStransky/pen/VKPVAG)

usage:
```
@include make-fixed-grid;

.page-nav{
  &.affix {
    @extend .col-xs-fixed-3;
    @extend .col-sm-fixed-3;
    @extend .col-md-fixed-3;
    @extend .col-lg-fixed-3;
    top: 20px;
    padding-left: 15px;
    padding-right: 15px;
  }
}
```

To add fixed widths to any child of a column
```
@include make-fixed-widths( '.affix' );
@include make-fixed-widths( '.affix-bottom' );
```
