# jQuery.clickable
###### Designed to make other elements clickable/tapable/pressable using its sibling or child links!

 - [View demo](http://lawlesscreation.github.io/jquery.clickable/)
 - [Download ZIP](https://github.com/lawlesscreation/jquery.clickable/archive/master.zip)

Built using the awesome [jQuery Boilerplate](https://github.com/jquery-boilerplate/boilerplate/) template.

## Requirements
 - [jQuery](http://jquery.com) >= v1.9.x

## Usage
Include the following scripts in your page, best at the bottom:
```html
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
  <script src="jquery.clickable.min.js"></script>
```

## Options &amp; defaults
<table>
  <thead>
    <tr>
      <th>Option</th>
      <th>Default</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>clickable_child</td>
      <td>null</td>
      <td>Used to make a child element clickable of which the script was executed</td>
    </tr>
    <tr>
      <td>select_link</td>
      <td>null</td>
      <td>Used to specify which link to use within the clickable box should more than one link be found</td>
    </tr>
    <tr>
      <td>clickable_class</td>
      <td>clickable</td>
      <td>The class that gets added to elements which have been successfully initialized</td>
    </tr>
    <tr>
      <td>hover_class</td>
      <td>clickable-hover</td>
      <td>The class that gets added to the onHover state of clickable elements</td>
    </tr>
    <tr>
      <td>focus_class</td>
      <td>clickable-focus</td>
      <td>The class that gets added to the onFocus state of clickable elements</td>
    </tr>
    <tr>
      <td>url_prefixes</td>
      <td>['http://', 'https://', 'www.']</td>
      <td>An array of different prefixes that can appear before each link</td>
    </tr>
  </tbody>
</table>

## Example: Link target
```javascript
$(function(){
  $('#clickable-box').find('.box').jqueryClickable();
});
```

## Example: Link image
```javascript
$(function(){
  $('#clickable-image').find('.box').jqueryClickable({
    clickable_child : 'img'
  });
});
```

## Example: Link image from heading
```javascript
$(function(){
  $('#clickable-image-from-heading').find('.box').jqueryClickable({
    clickable_child : 'img',
    select_link : 'h4'
  });
});
```

## Release history
 - 1.1.1 
 - 1.1.0 Changed to semantic versioning (2014-01-25)

Copyright &copy; 2013 [@lawlesscreation](http://twitter.com/lawlesscreation)

Licensed under [MIT](http://opensource.org/licenses/mit-license.php)


## TODO
 - Update to latest version of jQuery
 - Add Jasmine tests, JSLint
 - Add Callback to function
 - Add destroy function
