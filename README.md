## MOTHERSHIP a light & responsive stylus grid  
The intention of this grid is to give the developer the maximum amount of control over the customization of their grid, all it comes with are basic rows and columns. The thinking here is that you can take this grid and drop it anywhere and be using it in a very short amount of time.
### To fly the MOTHERSHIP 👽
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

_NOTE_: Columns are not pluralized, as it is silly, the `{NUMBER}` is the changeable element that will give the grid its direction. when you have two or more columns, obviously, you should use numbers that add up to the total number of your grid constant `GR = ...` illustrated below.

###### stylus:  
```js  
// CONSTANTS
  GR       = one two three...  
  WIDTH    = 100%
  MAXWIDTH = 1440px
  NUMBER   = length(GR)
  MARGIN   = 0.5%
```

_NOTE_: Constants you can do a good bit of customization on these variables, maybe all that you need, if not... You should make it code better for you! 😁

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
_...that will do the trick_  

### Credits
![Deep Space Nebula by:hameed@deviantart](http://pre09.deviantart.net/308d/th/pre/i/2010/032/9/b/deep_space_nebula_by_hameed.jpg)  
Image credit [hameed@deviantart](http://hameed.deviantart.com/)

### License
(The MIT License)

Copyright (c) Automattic <developer.wordpress.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.  


---  

_todo:_  
* clean up
* break stylus files into smaller bits (_ie. mixins, variables... etc._ )
