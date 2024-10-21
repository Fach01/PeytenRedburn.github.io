# PeytenRedburn.github.io
html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Background Image Slideshow</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body, html {
            height: 100%;
            font-family: Arial, sans-serif;
        }

        .slideshow-container {
            height: 100%;
            width: 100%;
            position: relative;
            overflow: hidden;
        }

        .slideshow-container::after {
            content: "";
            background-size: cover;
            background-position: center;
            background-image: url('image1.jpg');
            position: absolute;
            top: 0;
            left: 0;
            height: 100%;
            width: 100%;
            animation: fade 30s infinite;
        }

        @keyframes fade {
            0% { background-image: url('image1.jpg'); }
            25% { background-image: url('image2.jpg'); }
            50% { background-image: url('image3.jpg'); }
            75% { background-image: url('image4.jpg'); }
            100% { background-image: url('image1.jpg'); }
        }

        .content {
            position: relative;
            z-index: 1;
            color: white;
            text-align: center;
            padding-top: 20%;
        }

        h1 {
            font-size: 3rem;
        }

        p {
            font-size: 1.2rem;
        }
    </style>
</head>
<body>
    <div class="slideshow-container">
        <div class="content">
            <h1>Welcome to My Website</h1>
            <p>Enjoy the beautiful background transitions!</p>
        </div>
    </div>
</body>
</html>
