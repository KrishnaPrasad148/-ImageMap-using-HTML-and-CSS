# EX04 Simple Image Map using HTML & CSS
### DATE : 25/09/25

## AIM
To create a simple image map using HTML and CSS where different parts of an image are clickable, and clicking each part displays a message that highlights in green.



## DESIGN STEPS

### Step 1: 
- Add an image and link it to an image map using `usemap`.
- Define three clickable areas using `<area>` tags.
- Add three message boxes with IDs: `left`, `middle`, `right`.

### Step 2: 
- Style the image and message boxes.
- Use the `:target` selector to make the clicked message turn green.

### Step 3: 
- Click each image section and verify the correct box turns green.



## PROGRAM
```
Developed By :  Krishna Prasad S  
Register No. :  212223230108
```

###  index.html
```html
<!DOCTYPE html>
<html>
<head>
  <title>Simple Image Map</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>Simple Image Map</h1>
<p>Click any part of the image to see what area you clicked.</p>

<img src="https://images.unsplash.com/photo-1497752531616-c3afd9760a11?q=80&w=1170&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" usemap="#simplemap" class="map-img">

<map name="simplemap">
  <!-- Left Area -->
  <area shape="rect" coords="0,0,200,300" href="#left" alt="Left Area">
  <!-- Middle Area -->
  <area shape="rect" coords="200,0,400,300" href="#middle" alt="Middle Area">
  <!-- Right Area -->
  <area shape="rect" coords="400,0,600,300" href="#right" alt="Right Area">
</map>

<div id="left" class="box">You clicked the LEFT area.</div>
<div id="middle" class="box">You clicked the MIDDLE area.</div>
<div id="right" class="box">You clicked the RIGHT area.</div>

</body>
</html>

```

###  styles.css
```css
.map-img {
  width: 100%;
  max-width: 600px;
  border: 2px solid #333;
  display: block;
  margin-bottom: 20px;
}


.box {
  padding: 10px;
  background: #f2f2f2;
  border: 1px solid #aaa;
  margin-top: 10px;
  transition: 0.3s;
}

:target {
  background: #a8ffb3;
  border-color: #2f8f32;
}
```



## OUTPUT
<img width="1919" height="914" alt="left" src="https://github.com/user-attachments/assets/07464b97-2b46-4b63-827b-46a2ccfd122a" />
<img width="1919" height="914" alt="md" src="https://github.com/user-attachments/assets/c3f67093-d284-4989-a8c1-9fcd94ea098d" />
<img width="1919" height="920" alt="rght" src="https://github.com/user-attachments/assets/61bef3b9-60b5-47a9-9653-f7426ebd51fd" />


## RESULT
Thus a fully functional and simple **interactive image map** webpage is created using only **HTML and CSS**.






