
## Date:22/03/2025

## AIM
To create a interactive image gallery with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

### PROGRAM:

```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 20px;
            font-size: 24px;
            font-weight: bold;
        }
        .gallery-container {
            position: relative;
            width: 60%;
            margin: auto;
            overflow: hidden;
            background: white;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .gallery {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }
        .image-item {
            position: relative;
            min-width: 100%;
            overflow: hidden;
        }
        .image-item img {
            width: 80%;
            height: auto;
            border-radius: 8px;
            max-height: 300px;
        }
        .caption {
            position: absolute;
            bottom: 0;
            background: rgba(0, 0, 0, 0.7);
            color: white;
            width: 100%;
            text-align: center;
            padding: 10px;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        .image-item:hover .caption {
            opacity: 1;
        }
        .buttons {
            display: flex;
            justify-content: space-between;
            position: absolute;
            top: 60%;
            width: 100%;
            transform: translateY(-50%);
        }
        .btn {
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            font-size: 18px;
        }
        .btn:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }
        footer {
            margin-top: 20px;
            padding: 10px;
            background-color: #333;
            color: white;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <header>Welcome to My Site</header>
    <div class="gallery-container">
        <div class="gallery">
            <div class="image-item">
                <img src="naruto-1.webp" alt="Image 1">
                <div class=" caption">This arc is one of the earliest and most well-known, where Naruto Uzumaki joins Team 7 and they are sent on a mission to the Land of Waves. The episodes cover Naruto's growth and his team's struggles against the villain Gato, who threatens the village.</div>
            </div>
            <div class="image-item">
                <img src="naruto-3.webp" alt="Image 2">
                <div class=" caption">It follows the exploits of Naruto Uzumaki's son, Boruto Uzumaki, and his ninja team as they navigate their path in the ninja world. Initially, the manga retold the events of the film "Boruto: Naruto the Movie," but it later developed its own storyline focusing on Boruto's journey to become a great ninja and live outside his father's shadow</div>
            </div>
            <div class="image-item">
                <img src="naru-1.webp" alt="Image 3">
                <div class="caption">Throughout Naruto Shippuden, the themes of friendship, perseverance, and the pursuit of personal goals remain prominent, as the characters face numerous challenges and battles that test their resolve and abilities. Despite its length, the series is known for its engaging narrative and character development, making it a beloved continuation of the Naruto franchise.</div>
            </div>
        </div>
        <div class="buttons">
            <button class="btn" onclick="prevSlide()">&#10094; Prev</button>
            <button class="btn" onclick="nextSlide()">Next &#10095;</button>
        </div>
    </div>
    <footer> Ramprasath.R    212223220086</footer>

    <script>
        let index = 0;
        const gallery = document.querySelector('.gallery');
        const totalImages = document.querySelectorAll('.image-item').length;

        function showSlide() {
            gallery.style.transform = `translateX(${-index * 100}%)`;
        }
        function nextSlide() {
            index = (index + 1) % totalImages;
            showSlide();
        }
        function prevSlide() {
            index = (index - 1 + totalImages) % totalImages;
            showSlide();
        }
    </script>
</body>
</html>

```



## OUTPUT:
![Screenshot 2025-03-22 160504](https://github.com/user-attachments/assets/49366c20-10d6-4bb4-8139-390b1d1b3565)


## RESULT
The program for creating interactive image gallery using JavaScript is executed successfully.
![Screenshot 2025-03-22 160504](https://github.com/user-attachments/assets/2626b838-f0c0-4f96-8c96-a6be9230ba2a)
