Type: Template
Title: Landing Page Template


<!DOCTYPE html>
<html lang="en">
<head>
<title>laurel{separator}omg{separator}lol</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>
@import url('https://pvinis.github.io/iosevka-webfont/3.4.1/iosevka.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://fonts.googleapis.com/css2?family=Lily+Script+One&display=swap');

:root {
    --text:  #555;
}

* {
    box-sizing: border-box;
    margin: 0;
    font-family: 'Iosevka Web'
}

body {
    color: var(--text);
    size: 1em;
    background-color: #F5E0DC;
    max-width: 30em;
    margin: auto;
}

.top {
    top: 0;
    left: 0;
    position: sticky;
    background-color:#F5E0DC;
    max-width: 100%;
    height: 3.5rem;
}

.container {
    max-width: 30em;
    margin: auto;
}

.div {
    padding: 2rem;
    margin: 2rem;
    font-size: 0.9rem;
    background-color: white;
    border: 1px solid #000;
    z-index: 9999;
    box-shadow: 10px 10px;
}

.div-mini {
    border-top:4px solid #F5E0DC;
    border-top-style:dotted;
    padding-top: 1rem;
    padding-bottom: 1rem;
}

.message {
    background-color: white;
    border: 1px solid #000;
}

.center {
    text-align: center
}

nav ul {
  padding-top: 1rem;
  margin-left: -1rem;
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 2.5vmin;
  
  & > li {
    color: #313244;
    display: inline-flex;
    background:  #555;

    &:is(:hover, :focus-within) > button:not(:active) {
      --distance: -4px;
    }
  }
  
  & button {
    color: #777786;
    background-color: white;
    appearance: none;
    outline: none;
    font-size: 1rem;
    border: 1px solid #313244;

    --distance: 0;
    transform: translateX(var(--distance)) translateY(var(--distance));
    
    @media (prefers-reduced-motion: no-preference) {
      will-change: transform;
      transition: transform .2s ease ;
    }
  }
}

@media screen {
    .div {
        margin: 1rem;
        margin-bottom: 2rem;
    }
}

</style>
<div class="top">
    <nav class="links">
        <ul>
            <li><button>home</button></li>
            <li><button>posts</button></li>
            <li><button>now</button></li>
            <li><button>kudos</button></li>
        </ul>
    </nav>
</div>

<body>
    <div class="container">
    <div class="div">
        <div class="div-mini">
            <h2>@laurel</h2>
        </div>
        <div class="about">
            <div id="location" class="small"><i class="fa-solid fa-location-dot"></i> Mohkínstsis, Earth</div>
            <div id="education" class="small"><i class="fa-solid fa-graduation-cap"></i>
            School of Peer Support 2024</div>
            <br><br>
            <p>Plant-lovin' visionary type. Literary artist. YIMBY.  Unashamedly & unapologetically <i>pedestrian</i>. Answers promptly to the call of the afternoon daydream, the whistle of the tea kettle, or - sometimes - even the name Laurel. </p>
        </div>    
    </div>
    <div class="div">
        <div class="div-mini"></div>
        <p class="center">still adjusting some things around here - pls check back soon <i class="fa-regular fa-face-smile-beam"></i></p>
    </div>
</div>
</body>
</html>