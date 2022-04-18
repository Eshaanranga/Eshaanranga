- 👋 Hi, I’m @Eshaanranga
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Eshaanranga/Eshaanranga is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
---><html>
    <head>
        <Title>Session 27 And 26</Title>
    <style>
        body{
            background-color: antiquewhite;
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        text-align: center;
        }

    </style>
    </head>
<body>
    <h1>GEOLOCATION</h1>
<h2>04-09-22</h2>


<input type="button" value="Display my name" onclick="Display()">
<input type="button" value="Display My location" onclick="GetLocation()">
<p id="paragraph"></p>
</body>
<script>
    function Display(){
        var paragraph = document.getElementById("paragraph");
        paragraph.innerText = "Eshaan";
    }
    function GetLocation(){
        if(navigator.geolocation){
            paragraph.innerText = "Geolocation is available";
            navigator.geolocation.getCurrentPosition(showPosition);
        }
        else{
            paragraph.innerText = "Geolocation not available";
        }
        }

        function showPosition(position){
            paragraph.innerText = "Latiitude = " +position.coords.latitude+
            " Longitude = " +position.coords.longitude;
            
        }
    
</script>
</html>
