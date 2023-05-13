### Hi there 👋
![](https://github-readme-stats.vercel.app/api?username=1746705990)

<!DOCTYPE html>
<html>
<head>
    <title>IP Address and User Agent Info</title>
</head>
<body>
    <h1>IP Address and User Agent Info</h1>
    <p>IP Address: <span id="ip"></span></p>
    <p>Country: <span id="country"></span></p>
    <p>Operating System: <span id="os"></span></p>

    <script>
        // Get IP Address and Country
        fetch('https://ipapi.co/json/')
            .then(response => response.json())
            .then(data => {
                document.getElementById('ip').textContent = data.ip;
                document.getElementById('country').textContent = data.country_name;
            });

        // Get Operating System
        let os = "Unknown";
        if (navigator.appVersion.indexOf("Win") != -1) os = "Windows";
        if (navigator.appVersion.indexOf("Mac") != -1) os = "MacOS";
        if (navigator.appVersion.indexOf("X11") != -1) os = "UNIX";
        if (navigator.appVersion.indexOf("Linux") != -1) os = "Linux";
        document.getElementById('os').textContent = os;
    </script>
</body>
</html>

<!--
**1746705990/1746705990** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
