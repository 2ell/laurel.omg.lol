Type: Template
Title: Page Template


<!DOCTYPE html>
<html lang="en">
<head>
<title>{weblog-title}{separator}{post-title}</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
{feeds}
<style>
@import url('https://pvinis.github.io/iosevka-webfont/3.4.1/iosevka.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
</style>
<link rel="stylesheet" href="https://laurel.omg.lol/style.css">
</head>
<body>

    <div class="toggle">
        <div class="darkmode">
          <input type="checkbox" class="checkbox" id="checkbox">
          <label for="checkbox" class="label"></label>
            <div class="ball"></div>
          </label>
        </div>
      </div>

<header>
	<h1 class="weblog-title"><a href="{base-path}">{weblog-title}</a></h1>
	{navigation}
</header>

<main>

{body}

</main>

<footer>
    <p>created with <i class="fas fa-heart"></i> by laurel
        <br>
    <i class="fas fas fa-plug"></i> powered by <a href="https://omg.lol">omg.lol</a></p>
</footer>

<script>
      const checkbox =document.getElementById('checkbox')

checkbox.addEventListener('click',checkMode)

function checkMode(){
    if(checkbox.checked){
        darkModeOn()
    }else{
        darkModeOff()
    }
}

function darkModeOn(){
    document.body.classList.add('dark-mode')
}

function darkModeOff(){
    document.body.classList.remove('dark-mode')
}
</script>
</body>
</html>