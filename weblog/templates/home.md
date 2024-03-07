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
<span class="hide">proven.lol/8ab7de</span>

<div class="top">
    <div class="title-bar">
      <span class="weblog-title-sm"><a href="/">laurel.omg.lol</a>/{title}</span>
    </div>  
      <div class="dropdown">
            <a href="javascript:void(0);" class="icon" onclick="dropDown()">
                <i class="fa fa-bars"></i>
              </a>
              <div class="dropdown">
            <div id="navLinks">
                <ul>
                <li><a href="/">home</a></li> 
                <li><a href="/about">about</a></li>
                <li><a href="/noww">now</a></li>
                <li><a href="/kudos">kudos</a></li>
            </ul>
            </div>
            </div>
          </div> 
          <div class="toggle">
            <div class="darkmode">
              <input type="checkbox" class="checkbox" id="checkbox">
              <label for="checkbox" class="label"></label>
                <div class="ball"></div>
              </label>
            </div>
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
	<h1 class="weblog-title">laurel</h1>  
    <div id="location" class="small"><i class="fa-solid fa-location-dot"></i> Mohkínstsis, Earth</div>
    <div id="education" class="small"><i class="fa-solid fa-graduation-cap"></i>
        School of Peer Support 2024</div>
    <br><br>
        <p class="small"><i class="fa-solid fa-seedling"></i> Plant-lovin' visionary type. Literary artist. YIMBY.  Unashamedly & unapologetically <i>pedestrian</i>. Answers promptly to the call of the afternoon daydream, the whistle of the tea kettle, or - sometimes - even the name Laurel. Grateful to /still/ be here. <i class="fa-regular fa-face-smile-beam"></i></p>
    </div>
</div>
</header>
<main>
    <div class="connection">
        <div class="list1">
              <ul class="connect">
                <li>
                  <i class="fa-brands fa-mastodon"></i> <a rel="me" href="https://social.lol/@laurel">Mastodon</a>
                </li>
                <li>
                  <i class="fa-brands fa-lastfm"></i> <a rel="me" href="https://www.last.fm/user/laurel___">Last.fm</a>
                </li>
                <li>
                  <i class="fa-brands fa-github-alt"></i> <a href="https://github.com/2ell">Github</a>
                </li>
                <li>
                  <i class="fa-brands fa-discord"></i> <a rel="me" href="https://discordapp.com/users/susurrance">Discord</a>
                </li>
                </ul>
              </div>
                <div class="list2"><ul class="connect">
                <li>
                  <i class="fa-brands fa-steam"></i> <a rel="me" href="https://steamcommunity.com/id/2tongued/">Steam</a>
                </li>
                <li>
                  <i class="fa-solid fa-camera"></i> <a rel="me" href="https://pixey.org/i/portfolio/laurel">Pixelfed</a>
                </li>
                <li>
                  <i class="fa-solid fa-book"></i> <a href="https://bookrastinating.com/user/laurel"> Bookwyrm</a>
                </li>
                <li>
                  <i class="fa-solid fa-envelope"></i> <a rel="me" href="mailto:laurel@omg.lol">Email</a>
                </li>
              </ul></div>
            </div>
<div class="div-1">
<h4 style="font-family: var(--heading);">latest posts</h4>
    <div class="status">
        <script src="https://status.lol/laurel.js?time&link"></script>
    </div>    
        <div class="last-fm">
            <script src="https://recentfm.rknight.me/now.js?u=laurel___"></script>
            </div>

{body}
<hr>
</div>
</main>


<footer>
    <p>created with <i class="fas fa-heart" style="color: var(--pink);""></i> by laurel
        <br>
    <i class="fas fas fa-bolt" style="color: var(--yellow);"></i> powered by the wondrous <a href="https://omg.lol">omg.lol</a> <i class="fas fas fa-bolt" style="color: var(--yellow);"></i></p>
<div class="btns">
    <a href="https://ko-fi.com/s/4662b19f61"><img src="https://2ell.b-cdn.net/MadeByAHuman_08.png"></a> <a href="https://ko-fi.com/s/4662b19f61"><img src="https://2ell.b-cdn.net/NeverByAi_04.png"></a><br>
<img src="https://2ell.b-cdn.net/interoperability-pledge-an.gif"> <a href="https://archlinux.org/"><img src="https://2ell.b-cdn.net/arch-btn1.png"></a> <img src="https://2ell.b-cdn.net/furby.gif">
</div>
</footer>



<script>
function dropDown() {
    var x = document.getElementById("navLinks");
    if (x.style.display === "block") {
      x.style.display = "none";
    } else {
      x.style.display = "block";
    }
  } 

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