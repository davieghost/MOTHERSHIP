## light & responsive stylus grid  
The intention of this grid is to give the developer the maximum amount of control over the customization of their grid, all it comes with are basic rows and columns. The thinking here is that you can take this grid and drop it anywhere and be using it in a very short amount of time.
### grid use  
###### markup:
```html
<!-- rw stands for row. the row will hold your columns -->
<div class="rw">
  <!-- the number can be designated by you, the user, in the grid.styl file -->
  <div class="{NUMBER}-cl">
    {COLUMN CONTENT}
  </div>
</div>
```  
_note_: columns are not pluralized, as it is silly, the `{NUMBER}` is the changeable element that will give the grid its direction. when you have two or more columns, obviously, you should use numbers that add up to the total number of your grid constant `GR = ...` illustrated below.

###### stylus:  
```js  
// CONSTANTS
  GR       = one two three...  
  WIDTH    = 100%
  MAXWIDTH = 1440px
  NUMBER   = length(GR)
  MARGIN   = 0.5%
```
_note_:






_Initial set-up..._

```bash  
... $ npm install
... $ npm run build:stylus

```  
_If you want to make changes..._

```bash
... $ npm run build:stylus
```  
this will compile the `index.css` file from the `index.styl` file.  

_If you want to make live changes..._

```bash  
... $ npm run build:watch
```  
and this will compile the `index.css` file from the `index.styl` file as you save.  

packages:
* [_Stylus_](https://github.com/stylus/stylus)
* [_onchange_](https://github.com/Qard/onchange)
* [_watch_](https://github.com/mikeal/watch)

_All of these packages should **also** be installed globally_
```bash
... $ npm install stylus onchange watch-cli -g
```
___

_todo:_  
* ~~add margins~~  
* ~~modularize the customization of the grid (column amnt)~~  
* ~~create a README that is geared toward use of the gird (naming, etc...)~~  
* ~~refactor 'for loops'~~
