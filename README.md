# Build your dream apartment!

For this lab, use your imagination and your new AFrame skills to build out your dream apartment. A few fun models have been placed in the apartment to get you started.

You'll need to use planes and positioning to build the walls, floor, and ceiling. An example of a wall is included in `index.html`, but feel free to make your apartment bigger, smaller, or have multiple rooms.

### Downloading Models

You'll also want to add models to your apartment to make it look more realistic. You can download models from [Clara.io](https://clara.io/library) or [Google Poly Blocks](https://poly.google.com/) and use them in your project by including them as assets. 
 
```js
<!--Couch-->
<a-assets>
	<a-asset-item id="couch-obj" src="images/couch/couch.obj"></a-asset-item>
	<a-asset-item id="couch-mtl" src="images/couch/couch.mtl"></a-asset-item>
</a-assets>

```
 
And then using the asset ```id``` and as your ```a-obj-model ``` ```src``` and ```mtl```. Use scale, positioning and rotation to place your models in your apartment.

```js
<!--Couch-->
<a-obj-model src="#couch-obj" mtl="#couch-mtl" position="-23 -10 -8" scale="7 7 7"></a-obj-model>
```

### Using Google Poly

Alternatively, you can load models directly from Google Poly using an `a-entity` tag with the property of `gblock="url"`.

Nested within your `<head>` tags, make sure you have the following scripts loaded.

```js
<script src="https://aframe.io/releases/0.7.0/aframe.min.js"></script>
<script src="https://cdn.rawgit.com/archilogic-com/aframe-gblock/6498b71d/dist/gblock.js"></script>
```
Don't forget to use the properties of `position` or `scale` to help place your models!

```js
<!-- Edward Munch's The Scream artwork -->
<a-entity gblock="https://poly.google.com/view/ab0SP8HCU57"></a-entity>
```

This lab is open ended so feel free to get as imaginative a you want. Pinterest has some great [apartment inspo](https://www.pinterest.com/saraseven/tiny-apartment-inspiration/?lp=true). A dream apartment example can be found [here](https://melaniep518.github.io/dream-apt/).
