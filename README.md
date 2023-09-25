<!DOCTYPE html>
<html>
<head>
    <title>TRABELSSI Sejed</title>
    <style>
        body {
            background-color: black;
            color: white; /* Text color */
            font-family: Arial, sans-serif;
            margin: 0; /* Remove default margin */
            padding: 0; /* Remove default padding */
            text-align: center;
        }

        h1 {
            padding: 20px;
        }

        /* Style the download link */
        #downloadLink {
            display: none; /* Initially, hide the download link */
            text-align: center;
            padding: 10px;
            background-color: #333; /* Background color for the download link */
            color: white;
            text-decoration: none;
            border-radius: 5px;
            margin: 20px auto;
            width: 200px;
            display: block;
        }

        /* On hover, change background color */
        #downloadLink:hover {
            background-color: #555;
        }

        /* Style the countdown timer */
        #countdown {
            font-size: 24px;
            margin-top: 10px;
        }

        /* Style the additional text */
        #additionalText {
            font-size: 18px;
            margin-top: 20px;
        }
    </style>
    <script>
        function startCountdown() {
            var bouton = document.getElementById("boutonAfficher");
            bouton.style.display = "none"; // Hide the button

            var countdown = document.getElementById("countdown");
            countdown.style.display = "block"; // Show the countdown

            var additionalText = document.getElementById("additionalText");
            additionalText.style.display = "block"; // Show the additional text

            var seconds = 20; // Set the countdown duration (in seconds)

            var timer = setInterval(function () {
                countdown.textContent = seconds + " seconds remaining";
                seconds--;

                if (seconds < 0) {
                    clearInterval(timer); // Stop the timer
                    var lienDeTelechargement = document.createElement("a");
                    lienDeTelechargement.id = "downloadLink";
                    lienDeTelechargement.href = "https://github.com/TSSEJED/-/raw/main/%F0%9F%93%9A%F0%9F%95%8C%F0%9F%8C%9F%20%D8%A7%D9%84%D8%AA%D8%B1%D8%A8%D9%8A%D8%A9%20%D8%A7%D9%84%D8%A5%D8%B3%D9%84%D8%A7%D9%85%D9%8A%D9%91%D8%A9%20%F0%9F%93%9A%F0%9F%95%8C%F0%9F%8C%9F.docx%20(version%20publique).docx";
                    lienDeTelechargement.textContent = "Download the .docx file";
                    document.body.appendChild(lienDeTelechargement);
                    countdown.style.display = "none"; // Hide the countdown
                }
            }, 1000); // Update every 1 second (1000 milliseconds)
        }
    </script>
</head>
<body>
    <h1>TRABELSSI Sejed</h1>
    <div id="additionalText">

👋 Hello! I am TRABELSSI Sejed 👦 and I am 1️⃣4️⃣ years old. I am living in Tunisia 🇹🇳, specifically in Mannouba 🏘️, and I am studing at Marie Curie Academy 🏫. My birthday is on 25.05.2009 🎂🎉. I am passionate about learning and programming 🧵🛠️ 📚🧠 and have big dreams for the future 🌟✨.

</div>
    <button id="boutonAfficher" onclick="startCountdown()">Afficher mon lien</button>
    <div id="countdown" style="display: none;"></div>
</body>
</html># -
تربية اسلامية
