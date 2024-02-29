Type: Template
Title: Page Template


<!DOCTYPE html>
<html lang="en">
<head>
<title>laurel{separator}{post-title}</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
{feeds}
<style>
@import url('https://pvinis.github.io/iosevka-webfont/3.4.1/iosevka.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://fonts.googleapis.com/css2?family=Lily+Script+One&display=swap');
</style>
<link rel="stylesheet" href="https://laurel.omg.lol/style.css">
</head>
<body>
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
</header>

<main>
<h1 class="shadow" style="font-family: var(--heading); text-align: center;">{post-title}</h1>

<div class="content">
{body}
</div>

</main>

<footer>
    <p>created with <i class="fas fa-heart" style="color: var(--accent3);""></i> by laurel
        <br>
    <i class="fas fas fa-bolt" style="color: var(--accent)"></i> powered by the wondrous <a href="https://omg.lol">omg.lol</a> <i class="fas fas fa-bolt" style="color: var(--accent)"></i></p>
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