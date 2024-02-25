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
      <div class="nav">{navigation}</div>
</div>
</head>

<body>
<header>
    <div class="head-div">
        <div class="head-img">
    <img class="head-img" src="https://2ell.b-cdn.net/laureldark300.png">
</div>
<div class="title">
	<h1 class="weblog-title">laurel</h1>
        <p>Literary Artist. Dreamer. YIMBY.</p>
    </div>
</div>
<div class="div-1">
    <h1 style="text-align: right;">connect with me elsewhere</h1>
    <ul class="connect">
        <li>Mastodon</li>
        <li>Discord</li>
        <li>Pixey</li>
        <li>last.fm</li>
        <li>Bookwyrm</li>
    </ul>
</div>
</header>

<main>

{body}

<hr>

<div class="pagination">
{previous-page} {separator} {next-page}
</div>

</main>

<footer>
    <p>created with <i class="fas fa-heart"></i> by laurel
        <br>
    <i class="fas fas fa-plug"></i> powered by the wonderous <a href="https://omg.lol">omg.lol</a></p>
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