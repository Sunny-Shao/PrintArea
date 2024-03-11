[toc]
# jquery.PrintArea.js

Override the jQuery plugin written by Chris Ritschard.

## 1. Usage
``` js {.line-numbers}
/**
 *  Tested in Edge 122.0.2365.80, Safari 17.3, Firefox 123.0.1 and Chrome 122.0.6261.112
 *  Example:
 *      Print Button: <div id="print_button">Print</div>
 *      Print Area  : <div class="PrintArea" id="MyId" class="MyClass"> ... html ... </div>
 *      Javascript  : <script>
 *                       $("div#print_button").click(function(){
 *                           $("div.PrintArea").printArea( [OPTIONS] );
 *                       });
 *                     </script>
 *  options are passed as json (example: {mode: "popup", popClose: false})
 *
 *  {OPTIONS}   | [type]     | (default), values      | Explanation
 *  ---------   | ---------  | ---------------------- | -----------
 *  @mode       | [string]   | (iframe),popup,newtab  | printable window is either iframe or browser popup
 *  @popHt      | [number]   | (500)                  | popup window height
 *  @popWd      | [number]   | (400)                  | popup window width
 *  @popX       | [number]   | (500)                  | popup window screen X position
 *  @popY       | [number]   | (500)                  | popup window screen Y position
 *  @popTitle   | [string]   | ('')                   | popup window title element
 *  @popClose   | [boolean]  | (false),true           | popup window close after printing
 *  @tabClose   | [boolean]  | (true),false           | new tab close after printing
 *  @extraCss   | [string]   | ('')                   | comma separated list of extra css to include
 *  @retainAttr | [string[]] | ["id","class","style"] | string array of attributes to retain for the containment area. (ie: id, style, class)
 *  @standard   | [string]   | strict, loose, (html5) | Only for popup. For html 4.01, strict or loose document standard, or html 5 standard
 *  @extraHead  | [string]   | ('')                   | comma separated list of extra elements to be appended to the head tag
 */
```
## 2. Demo
*[Demo page](https://sunnyshao-print.netlify.app/index.html)* showcasing my plugin override and providing instructions on how to use it.

## 3. Reference
- *[PrintArea (by Chris Ritschard)](https://plugins.jquery.com/PrintArea)*
- *[Demo Page (by Chris Ritschard)](https://www.jqueryscript.net/demo/Print-Specified-Area-Of-A-Page-PrintArea/demo/)*