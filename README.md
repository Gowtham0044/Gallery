# Ex.07 Design of Interactive Image Gallery
# Date:28/05/2026
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>BMW Gallery</title>
    <style>
        body { margin: 0; display: flex; flex-direction: column; align-items: center; min-height: 100vh; font-family: sans-serif; color: #fff; background: #222; background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.8)), url('bmw_background.jpg') no-repeat center center fixed; background-size: cover; }
        h1 { margin: 40px 0 10px; letter-spacing: 5px; text-transform: uppercase; font-weight: 300; }
        .gallery-container { display: grid; grid-template-columns: repeat(5, 1fr); gap: 20px; width: 95%; max-width: 1200px; padding: 20px; }
        .gallery-item { border-radius: 12px; overflow: hidden; cursor: pointer; transition: 0.3s; border: 1px solid #444; background: rgba(255,255,255,0.05); text-align: center; }
        .gallery-item:hover { transform: translateY(-5px); border-color: #0066b3; box-shadow: 0 10px 20px rgba(0,0,0,0.5); }
        .gallery-item img { width: 100%; height: 160px; object-fit: cover; display: block; }
        .car-name { padding: 10px; margin: 0; font-size: 13px; letter-spacing: 1px; text-transform: uppercase; color: #ccc; }
        .overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.9); z-index: 10; justify-content: center; align-items: center; }
        .overlay img { max-width: 90%; max-height: 80%; border-radius: 8px; }
        .close { position: absolute; top: 20px; right: 30px; font-size: 40px; cursor: pointer; color: #fff; }
        footer { margin: auto 0 20px; color: #666; font-size: 12px; letter-spacing: 2px; text-transform: uppercase; }
    </style>
</head>
<body>

    <h1>BMW Theme Gallery</h1>

    <div class="gallery-container">
        <div class="gallery-item" onclick="openOverlay('bmw m3 cs.webp')">
            <img src="bmw m3 cs.webp">
            <p class="car-name">BMW M3 CS</p>
        </div>
        <div class="gallery-item" onclick="openOverlay('bmw m4 competition.webp')">
            <img src="bmw m4 competition.webp">
            <p class="car-name">M4 Competition</p>
        </div>
        <div class="gallery-item" onclick="openOverlay('bmw i8.webp')">
            <img src="bmw i8.webp">
            <p class="car-name">BMW i8</p>
        </div>
        <div class="gallery-item" onclick="openOverlay('bmw m3 gtr.webp')">
            <img src="bmw m3 gtr.webp">
            <p class="car-name">BMW M3 GTR</p>
        </div>
        <div class="gallery-item" onclick="openOverlay('BMW M4 CS.webp')">
            <img src="BMW M4 CS.webp">
            <p class="car-name">BMW M4 CS</p>
        </div>
    </div>

    <div id="overlay" class="overlay" onclick="this.style.display='none'">
        <span class="close">&times;</span>
        <img id="overlayImg">
    </div>

    <footer>Developed by Sharan</footer>

    <script>
        function openOverlay(src) {
            document.getElementById('overlayImg').src = src;
            document.getElementById('overlay').style.display = 'flex';
        }
    </script>

</body>
</html>
```
# OUTPUT:
<img width="1501" height="756" alt="image" src="https://github.com/user-attachments/assets/7b863f6e-934d-44d2-8889-ed875254681e" />

<img width="1438" height="795" alt="image" src="https://github.com/user-attachments/assets/c27e6641-70d9-4828-ace1-7be707c9ac12" />

<img width="1433" height="772" alt="image" src="https://github.com/user-attachments/assets/b78c4fda-8e8f-4f18-b81d-5b1255e95fbf" />

<img width="1393" height="691" alt="image" src="https://github.com/user-attachments/assets/a60be1f3-0b57-41d8-b9b7-2d58529c8c4e" />

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
