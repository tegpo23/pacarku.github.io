
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kolase Foto</title>
    <style>
        body {
            font-family: 'Courier New', Courier, monospace;
            background: linear-gradient(to bottom, #fbc2eb 0%, #a6c1ee 100%);
            color: #fff;
            text-align: center;
            padding: 20px;
            margin: 0;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 20px;
            text-shadow: 2px 2px #333;
        }
        .heart {
            color: red;
            animation: pulse 1s infinite;
        }
        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.1);
            }
            100% {
                transform: scale(1);
            }
        }
        .collage {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .collage img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            cursor: pointer;
        }
        .collage img:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
        }
        .caption {
            font-size: 1.5em;
            margin-top: 20px;
            text-shadow: 1px 1px #333;
        }
        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.9);
        }
        .modal-content {
            margin: auto;
            display: block;
            width: 80%;
            max-width: 700px;
        }
        .modal-content img {
            width: 100%;
            height: auto;
            border-radius: 10px;
        }
        .close {
            position: absolute;
            top: 20px;
            right: 35px;
            color: #fff;
            font-size: 40px;
            font-weight: bold;
            transition: 0.3s;
            cursor: pointer;
        }
        .close:hover,
        .close:focus {
            color: #bbb;
            text-decoration: none;
            cursor: pointer;
        }
        /* Background Music */
        #backgroundMusic {
            position: fixed;
            bottom: 10px;
            right: 10px;
            z-index: 2;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.8);
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
        }
        #backgroundMusic img {
            width: 30px;
            height: 30px;
        }
    </style>
</head>
<body>
    <h1>Pacar Cantikku <span class="heart">❤️</span></h1>
    <div class="collage">
        <img src="a1.jpg" alt="Photo 1" onclick="openModal(this)">
        <img src="a2.jpg" alt="Photo 2" onclick="openModal(this)">
        <img src="a3.jpg" alt="Photo 3" onclick="openModal(this)">
        <img src="a4.jpg" alt="Photo 4" onclick="openModal(this)">
        <img src="a5.jpg" alt="Photo 5" onclick="openModal(this)">
        <img src="a6.jpg" alt="Photo 6" onclick="openModal(this)">
        <img src="a7.jpg" alt="Photo 7" onclick="openModal(this)">
        <img src="a8.jpg" alt="Photo 8" onclick="openModal(this)">
        <img src="a9.jpg" alt="Photo 9" onclick="openModal(this)">
        <img src="a10.jpg" alt="Photo 10" onclick="openModal(this)">
        <img src="a11.jpg" alt="Photo 11" onclick="openModal(this)">
        <img src="a12.jpg" alt="Photo 12" onclick="openModal(this)">
    </div>
    <div class="caption"><h1>Kamu Selalu Cantik</h1></div>
</body>
</html>
