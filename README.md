# bootstrap3-fixed-width-columns
Generate classes for fixed width columns

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
```
