# lieber_saemi

<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>Lieber Sämi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 40px;
            background-color: #f4f4f4;
        }
        #text {
            font-size: 1.2em;
            white-space: pre-wrap;
        }
    </style>
</head>
<body>
    <div id="text"></div>
    <script>
        const message = "Lieber Sämi\n\nVielen Dank für die interessanten Gespräche über KI, Informatik und auch dein neues Spiel. Du hast das Interesse für diese Themen in mir wieder geweckt, das hat mich sehr gefreut.\n\nIch finde auch deinen Umgang und deine Art mit deinen Mitmenschen sehr toll und deine humorvolle Art hat mich schon das eine oder andere Mal zum Lachen gebracht.\n\nAuch finde ich deine direkte Art sehr angenehm. Ich freue mich, dich im nächsten Schuljahr ab und zu anzutreffen.\n\n01101100 01100111\n\nJannis";
        let i = 0;
        function typeWriter() {
            if (i < message.length) {
                document.getElementById("text").innerHTML += message.charAt(i);
                i++;
                setTimeout(typeWriter, 50);
            }
        }
        window.onload = typeWriter;
    </script>
</body>
</html>
