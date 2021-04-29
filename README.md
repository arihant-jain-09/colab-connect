<div align="center">
  
<h2>Stop Colab from Disconnecting</h2>

### Paste both the codes in console by Ctrl+Shift+I  then click console
</div>

<ul>
<li>Paste below code to click connect button every minute</li>

```js
function ClickConnect() {
  console.log('Working')
  document
    .querySelector('#top-toolbar > colab-connect-button')
    .shadowRoot.querySelector('#connect')
    .click()
}
intervalTiming = setInterval(ClickConnect, 60000)
```
<li>Below code add extra cells every minute you may alter this time </li>

```js
function ClickConnect(){
  console.log('Working');
  document.querySelector('colab-toolbar-button#toolbar-add-text').click();
}
intervalTiming = setInterval(ClickConnect, 60000);
```
</ul>


