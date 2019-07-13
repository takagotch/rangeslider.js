### rangeslider.js
---
https://github.com/andreruffert/rangeslider.js


```sh
bower install --save rangeslider.js
npm install --save rangeslider.js
```

```js
$('input[type="range"]').val(10).change();

$('input[type="range"]').rangeslider({
  polyfill: true,
  rangeClass: 'rangeslider',
  disabledClass: 'rangeslider--disabled',
  horizontalClass: 'rangeslider--horizontal',
  verticalClass: 'rangeslider--vertical',
  fillClass: 'rangeslider__fill',
  handleClass: 'rangeslider__handle',
  onInit: function(){};
  onSlide: function(position, value){},
  onSlideEnd: function(position, value){}
});
```

```
<input
  type="range"
  min="10"
  max="1000"
  step="10"
  value="300"
  data-orientation="vertical"
>

<script src="jquery.min.js"></script>
<script src="rangeslider.min.js"></script>
<script>
  $('input[type="range"]').rangeslider();
  $('input[type="range"]').rangeslider('destroy');
  $('input[type="range"]').rangeslider('update', true);
</script>
```



