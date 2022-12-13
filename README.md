# HTML
<!DOCTYPE html>
<html>
    <head>
        <title>Homepage</title>
    </head>
    <style>
        body{
            background-color: black;
            color: azure;
            font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        }
        .TitleBar{
            display: inline-grid;
            grid-template-columns: auto auto auto;
        }
        .dropdown{
            background-color: black;
            color: darkorange;
            font-size: 25px;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            font-weight: bold;
            border-block-color: black;
            border-color: black;
        }
        .logo{
            margin-left: 10px;
        
        }
        .NavigationBar{
            display:inline-grid;
            grid-template-columns: auto auto auto;
            padding: 25px 15px;
            margin: 0px 280px;
            width: 200px;
            align-items: center;
        }
        .NavigationElement{
            background-color: rgb(8, 0, 0);
            border: 5px solid black;
            padding: 5px 20px;
            font-size: 20px;
            color: deeppink;
        }
        #DM{
            margin-left: 0px;
        }
        a{color: orangered;}
        .open-button {
            background-color: orange;
            color: black;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            padding: 16px 20px;
            border: none;
            cursor: pointer;
            opacity: 0.7;
            position: fixed;
            top: 23px;
            right: 28px;
            width: 280px;
            }
        .form-popup {
                display: none;
                position: fixed;
                margin: auto;
                right: 15px;
                border: 3px solid darkgoldenrod;
        }
        .form-container {
            max-width: 300px;
            padding: 10px;
            background-color: rgb(8, 0, 0);
            color: orangered;
        }
        .form-container input[type=text], .form-container input[type=password] {
            width: 90%;
            padding: 15px;
            margin: 5px 0 22px 0;
            border: none;
            background: rgb(29,21,44);
        }
        .form-container input[type=text]:focus, .form-container input[type=password]:focus {
            background-color: black;
            color: azure;
            outline: none;
        }
        .form-container .btn {
            background-color: orange;
            color: white;
            padding: 16px 20px;
            border: none;
            cursor: pointer;
            width: 100%;
            margin-bottom:10px;
            opacity: 0.8;
        }
        .form-container .cancel {
            background-color: darkred;
        }
        .form-container .btn:hover, .open-button:hover{
            opacity: 1;
        }
        *{box-sizing:border-box}
        .slideshow-container {
        /* max-width: 450px; */
        position: relative;
        margin-left: auto;
        }
        .mySlides {
        display: none;
        }
        .prev, .next {
        cursor: pointer;
        position: absolute;
        top: 50%;
        width: auto;
        margin-top: -22px;
        padding: 16px;
        color: white;
        font-weight: bold;
        font-size: 18px;
        transition: 0.6s ease;
        border-radius: 0 3px 3px 0;
        user-select: none;
        }
        .next {
        right: 0;
        border-radius: 3px 0 0 3px;
        }
        .prev:hover, .next:hover {
        background-color: rgb(0,0,0);
        }
        .text {
        color: #f2f2f2;
        font-size: 15px;
        padding: 8px 12px;
        position: absolute;
        bottom: 8px;
        width: 100%;
        text-align: center;
        }
        .numbertext {
        color: #f2f2f2;
        font-size: 12px;
        padding: 8px 12px;
        position: absolute;
        top: 0;
        }
        .dot {
        cursor: pointer;
        height: 3px;
        width: 3px;
        margin: 0 2px;
        background-color: pink;
        border-radius: 50%;
        display: inline-block;
        transition: background-color 0.6s ease;
        }
        .active, .dot:hover {
        background-color: orangered;
        }
        .fade {
        animation-name: fade;
        animation-duration: 1.5s;
        }
        @keyframes fade {
        from {opacity: .4}
        to {opacity: 1}
        }
        .dot {
        width: 4px;
        height: 4px;
        margin-top: 10px;
        background-color: palevioletred;
        }
        .Location{
        text-align: left;
        font-style: inherit;
        font-size: 15px;
        color: darkorange;
        font-family: cursive;
        padding: 50px;
        background-color: black;
        width: 740px;
        height: 200px;
        }
        .Contact{
        padding: 50px;
        font-style: inherit;
        font-size: 15px;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        color: darkorange;
        background-color: black; 
        text-align: right;
        width: 740px;
        height: 200px;
        font-weight: bolder;
        }
        .ending{
            display: inline-grid;
            grid-template-columns: auto auto;
            border: 15px solid rgb(29,21,44);
        }
    </style>
    <script>
        function openForm() {
        document.getElementById("myForm").style.display = "block";
        }
        function closeForm() {
        document.getElementById("myForm").style.display = "none";
        }
        let slideIndex = 1;
        showSlides(slideIndex);

        // Next/previous controls
        function plusSlides(n) {
        showSlides(slideIndex += 1);
        }

        // Thumbnail image controls
        function currentSlide(n) {
        showSlides(slideIndex = 4);
        }

        function showSlides(n) {
        let i;
        let slides = document.getElementsByClassName("mySlides");
        let dots = document.getElementsByClassName("dot");
        if (n > slides.length) {slideIndex = 1}
        if (n < 1) {slideIndex = slides.length}
        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
        }
        for (i = 0; i < dots.length; i++) {
            dots[i].className = dots[i].className.replace(" active", "");
        }
        slides[slideIndex-1].style.display = "block";
        dots[slideIndex-1].className += " active";
        }

        funcion
    </script>
    <body>
        <div class="TitleBar">
            <div class="logo">
                <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\venkat.jpg" alt="Logo" width="150px">
            </div>
            <div class="NavigationBar">
                <div class="NavigationElement">
                    <select class="dropdown">
                        <option><a href="index.html"><h3>Home</h3></a></option>
                        <a href="https://www.google.com"><option><a href="https://www.google.com"><h3> xxxx</h3></a></option></a>
                        <option><a href="_"><h3>yyyy</h3></a></option>
                        <option><a href="_"><h3>zzzz</h3></a></option>
                        <option><a href="_"><h3>wwww</h3></a></option>
                    </select>
                </div>
                <div class="NavigationElement">
                    <select class="dropdown">
                        <option><a href="_"><h3>!!!!</h3></a></option>
                        <option><a href="_"><h3>@@@@@</h3></a></option>
                        <option><a href="_"><h3>####</h3></a></option>
                        <option><a href="_"><h3>$$$$</h3></a></option>
                        <option><a href="_"><h3>%%%%</h3></a></option>
                    </select>
                </div>
                <div class="NavigationElement">
                    <select class="dropdown">
                        <option><a href="_"><h3>+++++</h3></a></option>
                        <option><a href="_"><h3>^^^^^</h3></a></option>
                        <option><a href="_"><h3>&&&&&</h3></a></option>
                        <option><a href="_"><h3>*****</h3></a></option>
                    </select>
                </div>
            </div>
            <div class="Login-popup">
                <button class="open-button" onclick="openForm()">Open Form</button>
                <div class="form-popup" id="myForm">
                    <form class="form-container">
                    <h1>Login</h1>
                    <label for="email"><b>Email</b></label>
                    <input type="text" placeholder="Enter Email" name="email" required>
                    <label for="psw"><b>Password</b></label>
                    <input type="password" placeholder="Enter Password" name="psw" required>
                    <button type="submit" class="btn">Login</button>
                    <button type="button" class="btn cancel" onclick="closeForm()">Close</button>
                    </form>
                    
                </div>
            </div>  
        </div>
        <div class="TitleBar">
                <div id="DM">
                    <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\DigitalMarketing.jpg" alt="Digital Marketing" height="250px">
                </div>
                <div class="slideshow-container">
                    <div class="mySlides fade">
                        <div class="numbertext">1 / 4</div>
                        <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\Website1.webp" style="width:100%">
                        <div class="text">Caption Text</div>
                    </div>
                    <div class="mySlides fade">
                        <div class="numbertext">2 / 4</div>
                        <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\Website5.webp" style="width:100%">
                        <div class="text">Caption Two</div>
                    </div>
                    <div class="mySlides fade">
                        <div class="numbertext">3 / 4</div>
                        <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\Website4.jpg" style="width:100%">
                        <div class="text">Caption Three</div>
                    </div>
                    <div class="mySlides fade">
                        <div class="numbertext">4 / 4</div>
                        <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\Website3.webp" style="width:100%">
                        <div class="text">Caption Three</div>
                    </div>
                    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
                    <a class="next" onclick="plusSlides(1)">&#10095;</a>
                </div>
                <div id="Map">
                <img src="C:\Users\acer\Desktop\ \venkat'sWebsite\map1.PNG" alt="Map" width="400px" height="250px">
                </div>
            
        </div>
          <br>
        <div style="text-align:center">
            <span class="dot" onclick="currentSlide(1)"></span>
            <span class="dot" onclick="currentSlide(2)"></span>
            <span class="dot" onclick="currentSlide(3)"></span>
            <span class="dot" onclick="currentSlide(4)"></span>
        </div>
            <br>
        <div>
            <iframe src="C:\Users\acer\Desktop\ \venkat'sWebsite\Marketing Is Everything.pdf" title="Marketing is everything" width="50%" height="350px">Marketing is everything</iframe>
            <iframe src="C:\Users\acer\Desktop\ \venkat'sWebsite\GoodLeaderinBadEconomy.pdf" title="How to Be a Good Leader in Bad Ecomomy?" width="49%" height="350px">How to Be a Good Leader in Bad Ecomomy?</iframe>
        </div>
        <div class="ending">
            <div class="Location"><h3>Location:</h3>
                <p>Lovely Professional University Jalandhar </p>
                <p>New Delhi Road,</p>
                Phagwara
                Punjab 144001
            </div>
            <div class="Contact"> <h3>Contact: </h3>
                <p>Email: Shubham30p@gmail.com</p>
                <p>LinkedIn: linkedin.com/in/NewbieShubham</p>
                <p>Current Address: Jalandhar, Phagwara, LPU BH1 Room no. 718</p>
            </div>
        </div>


    </body>
</html>
