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
    
:root {
    --text: #313244;
    --link: #B4BEFE;
    --link-u: #B4BEFE;
    --link-hov:  #74C7EC;
    --background: #D9E0EE;
    --background-alt: #181825;
    --base: #313244;
    --foreground: #D9E0EE;
    --accent: #B4BEFE;
    --accent2: #94E2D5;
    --accent3: #F5C2E7;
    --surface:  #313244;
    --faint: #707880;
    --transparent: #00000000;
    --label: #89DCEB;
    --gradient: linear-gradient(60deg, var(--blue), var(--sky), var(--teal));

    --rosewater: #F5E0DC;
    --flamingo: #F2CDCD;
    --pink: #F5C2E7;
    --mauve: #CBA6F7;
    --red: #F38BA8;
    --maroon: #EBA0AC;
    --peach: #FAB387;
    --yellow: #F9E2AF;
    --green: #A6E3A1;
    --teal: #94E2D5;
    --sky: #89DCEB;
    --sapphire: #74C7EC;
    --blue: #89B4FA;
    --lavender: #B4BEFE;
}

.dark-mode {
    --link: #B4BEFE;
    --link-u: #B4BEFE33;
    --link-hov: #74C7EC66;
    --base: #1e1e2e;
    --background: #24273a;
    --accent: #B4BEFE33;
    --accent2: #94E2D533;
    --accent3: #F5C2E733;
    --background-alt: #181825;
    --surface:  #313244;
    --foreground: #D9E0EE;
    --text: #CDD6F4;
    --subtext1: #BAC2DE;
    --faint: #707880;
    --transparent: #00000000;
    --label: #F9E2AF;
    --gradient: linear-gradient(60deg, var(--yellow), var(--pink), var(--peach));

    --rosewater: #F5E0DC;
    --flamingo: #F2CDCD;
    --pink: #F5C2E7;
    --mauve: #CBA6F7;
    --red: #F38BA8;
    --maroon: #EBA0AC;
    --peach: #FAB387;
    --yellow: #F9E2AF;
    --green: #A6E3A1;
    --teal: #94E2D5;
    --sky: #89DCEB;
    --sapphire: #74C7EC;
    --blue: #89B4FA;
    --lavender: #B4BEFE;
}

* {
	box-sizing: border-box;
    margin: 0;
}

body {
	font-size: 1.2em;
	color: var(--text);
	background: var(--background);
    font-family: 'Iosevka Web', monospace;
}

p, li {
    line-height: 1.5rem;
    margin-bottom: 1em;
}


/* Link Styles */
a {
    color: var(--text);
    text-decoration: underline;
    text-decoration-color: var(--link-u);
    text-decoration-thickness: 0.4rem;
    text-decoration-skip-ink: none;
    text-underline-offset: -0.20rem;
    transition: text-decoration 0.3s ease;
}

/* Hover Styles for Links */
a:hover {
    text-decoration-color: var(--link-hov);
}

.large {
    font-size: 3em;
}

.small {
    font-size: 0.8em;
}

.hide {
    display: none;
}

/* Top Bar Styles */
.top {
  position: sticky;
  top: 0;
  left: 0;
  margin: 0;
  width: 100%;
  height: 4.5rem;
  background-color: var(--base);
  z-index: 10000;
}

/* Weblog Title Styles */
.top .weblog-title-sm a {
  font-size: 1em;
  color: var(--accent);
  margin-left: 0.5rem;
  margin-top: 2rem;
  text-decoration-color: var(--transparent);
  font-family: 'Lily Script One';
}

/* Navigation Links Styles */
.top #navLinks {
  display: none;
  position: relative;
  padding-top: 2rem;
  max-width: 20%;
  background-color: var(--base);
  transition: all 0.5s ease-in-out;
}

.top #navLinks ul {
  list-style: none;
  padding: 0.5rem;
}

.top #navLinks ul li {
  margin-top: 0.5rem;
}

.top #navLinks ul li a {
  display: block;
  padding: 0.2rem;
  padding-left: 1rem;
  color: var(--link);
  text-decoration: none;
  cursor: pointer;
}

.top #navLinks ul li a:hover {
  background-color: var(--background-alt);
  transition: all 0.2s ease-in-out;
}

/* Navigation Icon Styles */
.top a.icon {
  position: absolute;
  left: 1.5rem;
  top: 2rem;
  font-size: 1.2em;
  color: var(--background);
  display: block;
  z-index: 10;
}

.top a.icon:hover,
.top a.icon:active {
  color: var(--accent);
}

/* Toggle Styles */
.toggle {
    width: 3rem;
    position: absolute;
    top: 0.8rem;
    right: 0.5rem;
}

/* Label Styles */
.label {
    width: 2rem;
    height: 1rem;
    border-radius: 30px;
    background: var(--gradient);
    position: absolute;
    cursor: pointer;
}

/* Label Before Styles */
.label:before,
.label:after {
    content: '';
    position: absolute;
    display: inline-block;
}

/* Checkbox Checked Styles */
#checkbox:checked ~ .ball {
    transform: translateX(1rem);
}

/* Checkbox Styles */
#checkbox {
    display: none;
}

/* Ball Styles */
.ball {
    width: 0.7rem;
    height: 0.7rem;
    background-color: var(--surface);
    position: absolute;
    border-radius: 50%;
    margin-top: 2px;
    margin-left: 3px;
    cursor: pointer;
    transition: all 250ms ease-in-out;
}


main {
    max-width: 30em !important;
    margin: auto;
}

.div-1 {
    padding: 1rem;
}

.connection {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    justify-items: center;
    gap: 5rem;
    width: 100%;
    margin: auto;
}

.list1 {
flex-grow:1;
}

.list2 {
  flex-grow: 1;
}

.connect {
    list-style: none;
}

.statuslol {
        font-size: 0.8em;
        color: var(--accent3);
        background-color: var(--transparent);
        padding: 0em !important;
        margin: 0em !important;
        display: inline !important;
        overflow-wrap: break-word !important;
    }
    .statuslol_content {
        color: var(--text) !important;
        font-size: 0.8em;
        display: inline !important;
    }
    .statuslol_content p {
        display: inline !important;
    }
    .statuslol_time {
        display: inline !important;
        padding: 0 !important;
        font-weight: 600;
    }
    .statuslol_time a::before {
        font-weight: normal;
    }
    .statuslol_time a {
        font-size: 0.8em;
        text-decoration-color: var(--link-u);
        border: 1px solid var(--accent);
        padding: 0.2rem;
    }
    .statuslol_time a:hover {
        text-decoration-color: var(--link-hov);
    }
    .statuslol_emoji_container {
        display: inline !important;
    }
    .statuslol_emoji {
        max-width: 1em;
        max-height: 1em;
    }

.recent-played {
    color: var(--text);
    font-size: 0.8em;
    width: 100%;
    padding: 0;
}
.recent-played-track {
    padding-left: -1rem;
}

.recent-played-track a {
    font-size: 0.8em;
    padding-left: 0.1rem;
    text-decoration: none;
}

/* Common Styles for Header and Main */
header,
main {
    max-width: 60em;
    margin: auto;
}

/* Header Specific Styles */
header {
    margin-top: 0;
    margin-bottom: 0;
}

/* Header Container Styles */
.head-div {
    margin-top: 2em;
    overflow: visible;
    max-height: 35em;
    margin: auto;
    background-color: var(--background);
    display: flex;
    gap: 0rem;
    padding-bottom: 2rem;
}

.weblog-title {
    font-size: 5em;
    text-shadow: 3px 1px 1px var(--base), 2px 2px 1px var(--yellow), 4px 2px 1px #f5eee6,
    3px 3px 1px var(--teal), 5px 3px 1px #f5eee600;
}

.title {
    flex-shrink: 2;
    margin-top: 2rem;
    margin-right: 2rem;
}

#location, #education {
    display: inline;
    padding: 0.5rem;
    background-color: var(--background);
}

.dark-mode #location, .dark-mode #education {
    background-color: var(--transparent);
}

/* Image Styles */
.head-img,
.dark-mode .head-img {
    opacity: 1;
    margin-left: 1rem;
    max-width: 80%;
}

/* Hover Styles for Image */
.head-img:hover,
.dark-mode .head-img:hover {
    opacity: 1;
}

.status, .last-fm {
    margin: 1rem;
    border: 1px dotted #444;
    padding: 1rem;
}
/* Footer Styles */
footer {
    background: var(--base);
    color: var(--foreground);
    margin-top: 1rem;
    padding: 1em;
    font-size: 90%;
    text-align: center;
    border-top: 1px solid var(--accent);
}

/* Footer Link Styles */
footer a {
    color: var(--link);
    font-weight: 700;
    text-decoration: none;
    transition: color 0.3s ease; /* Consolidated transition properties */
}

footer a:hover {
    color: var(--sky);
}

/* Button Container Styles */
footer .btns {
    margin: 0.5rem auto; /* Consolidated margin properties */
    max-width: 80%;
}


@media only screen and (max-width: 600px) {
    body {
        font-size: 1em;
    }
    .content {
        text-align: left;
        margin-left: 0.5rem;
        margin-right: 0.5rem;
        text-justify: newspaper;
        hyphens: manual;
        hyphenate-character: '-';
    }
    .head-div {
        flex-direction: column;
        justify-content: center;
        margin-bottom: 0;
        padding-bottom: 2rem;
        padding-left: 0.5rem;
        padding-right: 0.5rem;
        max-height: fit-content;
    }
    #location, #education {
        display: block;
    }
    .head-img, .dark-mode .head-img {
        max-width: 15em;
        flex-shrink: 1;
        height: auto;
        margin: auto;
    }
    .connection {
      flex-direction: row;
      gap: 0rem;
      padding: 0rem;
      width: 100%;
      margin: 0, auto;
      font-size: 0.9rem;
    }
    .title {
        margin-top: -10em;
        margin-left: 1rem;
        margin-bottom: 1rem;
        text-align: center;
    }
    .title-bar {
        display: none;
    }
    .weblog-title {
        text-align: center;
        margin-left: 0em;
    }
    .top {
        max-height: 2rem;
    }
    .top a.icon {
        top: 0.2rem;
        left: 1rem;
    }
    .top #navLinks {
        padding-top: 2rem;
        max-width: 100%;
    }
    .toggle {
        top: 0.5rem;
    }
}



.home-post {
    display: flex;
    background-color: var(--background-alt);
    border-left: 4px solid {color};
    align-items: stretch;
    gap: 0;
    padding: 1rem;
    margin: 1rem;
}

.home-post > div {
    padding: 0.1rem;
}

.home-post-header {
    padding: 0.5rem;
    flex-grow: 1;
}

.home-post-image img {
    flex-shrink: 1;
    padding: 0em;
    align-self: flex-start;
    max-width: 15em;
}

.home-post-title {
    padding: 1rem;
    color: {color};
    text-align: left;
}

.home-post-info {
    font-size: 0.8em;
    margin-top: 1rem;
    margin-bottom: 0.5rem;
    text-align: right;
}

.home-post-type::before {
    font-family: 'Font Awesome 5 Free';
    content: '\{fa} ';
    margin-right: .2rem;
    padding-left: .5rem;
}

.home-post-type {
    display: block;
    margin-bottom: 1rem;
    font-size: 0.8rem;
    color: {color};
    border-radius: 10px;
    max-width: fit-content;
    padding: .2rem;
}

@media only screen and (max-width: 480px) {
    /* For mobile phones: */
    .home-post {
        flex-direction: column;
        align-items: normal;
    }
    .home-post-title {
        padding: 0;
    }
    .home-post-image {
        padding: 0.5rem;
        margin: auto;
    }
    .home-post-image img {
        max-width: 100%;
        margin: auto;
    }
}
</style>

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
    <div class="status">
        <script src="https://status.lol/laurel.js?time&link"></script>
    </div>    
        <div class="last-fm">
            <script src="https://recentfm.rknight.me/now.js?u=laurel___"></script>
            </div>

<div class="div-1">
<h4 style="font-family: var(--heading);">latest posts</h4>
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