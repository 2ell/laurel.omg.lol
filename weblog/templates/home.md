Type: Template
Title: Landing Page Template

<!DOCTYPE html>
<html lang="en">
<head>
<title>laurel{separator}omg{separator}lol</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
{feeds}
<style>
@import url('https://pvinis.github.io/iosevka-webfont/3.4.1/iosevka.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://fonts.googleapis.com/css2?family=Lily+Script+One&display=swap');
</style>
<link rel="stylesheet" href="https://laurel.omg.lol/style.css">

<head>

<div class="top">
    <div class="toggle">
        <div class="darkmode">
          <input type="checkbox" class="checkbox" id="checkbox">
          <label for="checkbox" class="label"></label>
            <div class="ball"></div>
          </label>
        </div>
      </div>

      <div class="nav"><span class="weblog-title-sm"><a href="/">laurel.omg.lol</a></span>
        <ul class="nav">
            <li><a href="/">home</a></li> 
            <li><a href="/about">about</a></li>
            <li><a href="/noww">now</a></li>
            <li><a href="/kudos">kudos</a></li>
        </ul>
    </div>
</div>
</head>

<body>
<header>
    <div class="head-div">
        <div class="head-img">
    <img class="head-img" src="https://2ell.b-cdn.net/2ell2dark.png">
</div>
<div class="title">
	<h1 class="weblog-title">laurel <i style="color: var(--accent);" class="fas fa-badge-check"></i></h1>
    <br><i class="fa-solid fa-location-dot"></i> Moh'kinsstis, Earth
    <br><i class="fa-solid fa-graduation-cap"></i> School of Peer Support 2024
    <br><br>
        <p>Plan[e]t-lovin' visionary type. Literary artist. YIMBY. Unashamedly & unapologetically <i>pedestrian</i>. Grateful to (still) be here.</p>
    </div>
</div>
<div class="div-1">
    <h1 style="font-family: var(--heading);">connect with me</h1>
    <ul class="connect">
              <li>
                <span class="fa-li"><i class="fa-brands fa-mastodon"></i></span><a rel="me" href="https://social.lol/@laurel">Mastodon</a>
              </li>
              <li>
                <span class="fa-li"><i class="fa-brands fa-discord"></i></span><a rel="me" href="https://discordapp.com/users/susurrance">Discord</a>
              </li>
              <li>
                <span class="fa-li"><i class="fa-solid fa-camera"></i></span><a rel="me" href="https://pixey.org/laurel">Pixelfed</a>
              </li>
              <li>
                <span class="fa-li"><i class="fa-brands fa-lastfm"></i></span><a rel="me" href="https://www.last.fm/user/laurel___">Last.fm</a>
              </li>
              <li>
                <span class="fa-li"><i class="fa-brands fa-steam"></i></span><a rel="me" href="https://steamcommunity.com/id/2tongued/">Steam</a>
              </li><br>
              <li>
                <span class="fa-li"><i class="fa-solid fa-envelope"></i></span><a rel="me" href="mailto:laurel@omg.lol">Email</a>
              </li>
            </ul>
    </ul>
</div>
</header>

<main>
<div class="div-2">
    <h1 style="font-family: var(--heading);">read my mind</h1>
{body}
<hr>
</div>
</main>

<footer>
    <p>created with <i class="fas fa-heart"></i> by laurel
        <br>
    <i class="fas fas fa-plug" style="color: var(--color1)"></i> powered by the wonderous <a href="https://omg.lol">omg.lol</a></p>
</footer>

<script>
const checkbox =document.getElementById('checkbox')

checkbox.addEventListener('click',checkMode)

                      function checkMode() {
                            if (localStorage.getItem('isDarkMode')=='true'){
                                localStorage.setItem('isDarkMode', false)} 
                                else 
                                {localStorage.setItem('isDarkMode', true)}
                                toggle();
                        };

                        function toggle(){
                            if (localStorage.getItem('isDarkMode')=='true'){
                            
                                document.body.classList.add('dark-mode');
                        }
                        if (localStorage.getItem('isDarkMode') === 'false'){
                                
                            document.body.classList.remove('dark-mode');
                            };
                        }
                        toggle()
</script>
</body>
</html>