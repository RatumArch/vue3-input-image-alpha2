# vue3-image-input

File input for Vue 3.
=======
This enhanced file input enable to pick a file with a preview.

Support preview for :
* **Image** : jpg, png, svg...
* **Video** : preview for mp4, webm and all other browser compatible format
* **Audio**
* **PDF**


<img src="./media/Screenshot_21.png" width="300" alt="Screenshot de présentation" >

# Install
```
npm i vue3-image-input
```
# Usage
1.  Import the *ImageInput* component
```js
import { ImageInput } from 'vue3-image-input'
```
2. Import style.css
      * in style block of your SFC (don't work with *scoped* attribute).
        ```css
        @import '/node_modules/vue3-image-input/dist/style.css';
        ```
      * or in the ```<script setup>```
        ```js
        import '/node_modules/vue3-image-input/dist/style.css'
        ```
If you don't import the built-in CSS, the components will not be ergonomic and you will have to write your custom CSS

## Exemple in a SFC

```html
<template>
  <!-- an-app.vue -->
  <h2>Upload a picture</h2>
  
  
  <ImageInput 
      format="large"
      textPlaceholder="Have you a picture ?"
      resizable
      class="a-class" />

  <button type="submit">Submit</button>
</template>
```

```css
<style >
/* an app.vue */
@import '/node_modules/vue3-image-input/dist/style.css';

.a-class {
  width: 200px;
  height: 400px;
  background-color: #ef0d50;
}
.a-class .preview {
  background-color: #e1f2f7;
  margin-top: 20px;
}

```

# Props
* ## accept
  * default value : ```"image/*, audio/*, video/*"```
  * type: ```string```
* ## imagePlaceholder
  Custom image
  * default value : built-in cover image

# Licence
MIT
