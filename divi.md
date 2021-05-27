# Tutorial for Divi

## Vertical center of content within a row

In order to align the content vertically you must :
1. Configure the row setting so it will adjust the height of the columns to be the same: design > sizing > Equalize Column Heights
2. Add the "vertical_center" class on all columns which you want to vertical center
3. Add the following CSS custom code to your template :
```css
/* Vertically center text */
/* Only select the columns with both et_pb_column & vertical_center class within a tag with a class of et_pb_equal_columns */
.et_pb_equal_columns > .et_pb_column.vertical_center {
  margin-top:auto;
  margin-bottom:auto
}
```