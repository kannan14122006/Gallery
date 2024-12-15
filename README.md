![Screenshot 2024-12-15 230820](https://github.com/user-attachments/assets/43b171e2-9521-4a31-be8d-eb49d72e4ad5)# Ex.08 Design of Interactive Image Gallery
# Date: 14/12/2024
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
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        #flexbox
        {
            padding: 170px;
            background-repeat: no-repeat;
            background-size: cover;
        }
        
        #container
        {
            gap: 20px;
            display: flex;
            justify-content: center;
            padding: 10px;
            box-shadow:0 2px 3px;
        }
        .img
        {
            height: 300px;
            width: 300px;
            /* transform: rotate(-10deg); */
            image-rendering:optimizeQuality;    
            border: 2px inset whitesmoke;    
            border-radius: 10px;
            box-shadow:  0 0 10px black ;
            transition: 0.5s;
        }
        .img:hover
        {
            content: 'hello';
            transform: scale(1.3);
        }
        #divs
        {
            display: inline;
        }
        #image
        {
            z-index: 100;
            display: none;
            background: rgba(0,0,0,0.5);
            position: fixed;
            width: 100%;
            /* transform: rotate(20deg); */
            height: 100%;
            top: 0;
            bottom: 0;
            align-items: center;
            justify-content: center;    
        }
        #image img{
            width: 600px;
            height: auto;
        }
        
    </style>
</head>
<body>
    <section id="image">
            <img src="1.jpeg" alt="" id="display" onclick="closes()">
    </section>
<div id="flexbox">

    <h1 align="center" ><span id="title">My Image Gallery </span></h1>

    <div id="container">
        <div class="divs"><img class="img" src="1.jpg" onclick="opens(this.src)" alt=""></div>
        <div class="divs"><img class="img" src="2.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs"><img class="img" src="3.jpg"  onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="4.jpg" onclick="opens(this.src)"   alt=""></div>
    </div>
    <div id="container">
        <div class="divs" ><img class="img" src="5.jpg" onclick="opens(this.src)"  alt=""></div>
        <div class="divs"><img class="img" src="6.jpg" onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="7.jpg" onclick="opens(this.src)"  alt=""></div>
       <div class="divs"><img class="img" src="8.jpg" onclick="opens(this.src)"  alt=""> </div>
    </div>
    
</div>
<footer align="center" style="background-color:grey">
    <p>Designed & Developed by Kannan &copy; </p>
</footer>
    <script>
            var a =document.getElementById("image");
            var b=document.getElementById("display");
            function opens(c)
            {
                a.style.display='flex';
                b.src=c;
            }
            function closes()
            {
                a.style.display='none';
            }
    </script>
</body>
</html>
```
# OUTPUT:
![Screenshot 2024-12-15 230820](https://github.com/user-attachments/assets/88768dce-b1c6-4440-8f6f-916497dd1729)
![Screenshot 2024-12-15 230830](https://github.com/user-attachments/assets/fc838286-ac62-49d4-b490-a3aed4dcd143)
![Screenshot 2024-12-15 230836](https://github.com/user-attachments/assets/943c39dc-89ab-4d7b-b35d-05f916c3e5b5)
![Screenshot 2024-12-15 230842](https://github.com/user-attachments/assets/748d5fbb-9b5c-4c7a-84b3-d22f90603429)
![Screenshot 2024-12-15 230850](https://github.com/user-attachments/assets/10e34de6-5411-47c9-bd11-9fe782ab2e80)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
