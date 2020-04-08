# docsify-twemoji

![](http://image.taqini.space/img/20200408231432.png)

Parse twitter style emoji in your docs. Chinese docs: [中文文档](http://taqini.space/2020/04/08/docsify-plugins/#twemoji)

## Feature of twemoji

- parse unicode emoji instead of `:tag:`
- large amount of emoji supported even full emoji

## Demo

You can see the demo of docsify-twemoji [here](http://note.taqini.space/) 

The [demo](http://note.taqini.space/)  site has also installed another plugins [docsify-livere](https://github.com/TaQini/docsify-livere)

![](http://image.taqini.space/img/20200408220415.png)



## Install

Add the docsify-twemoji plugin to your `index.html` after docsify.

```html
<!-- twemoji -->
<script src="//cdn.jsdelivr.net/gh/TaQini/docsify-twemoji@master/twemoji.min.js"></script>
```

Then include the following js code in the appropriate location on the `index.html`

```javascript
  window.$docsify = {
      plugins: [
        function (hook, vm) {
          // parse twemoji
          hook.doneEach(function() {
              twemoji.parse(document);
          });
        },
      ]
  }
```

## Usage

You can find various of emoji from [here](https://emojipedia.org/) or other place.

![](http://image.taqini.space/img/20200408215449.png)

Click the button to copy unicode of emoji to your clip board and then paste it into your docs.

For example `😀` will be parsed to <img src="https://twemoji.maxcdn.com/v/12.1.5/72x72/1f600.png" alt="happy" style="zoom:25%;" />

