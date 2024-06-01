Type: Template
Title: Landing Page Template


<!DOCTYPE html>
<html lang="en">
<head>
<title>laurel{separator}omglol</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>
@import url('https://pvinis.github.io/iosevka-webfont/3.4.1/iosevka.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://fonts.googleapis.com/css2?family=Inclusive+Sans:ital@0;1&display=swap');

:root {
    --text: #cdd6f4;
    --subtext: #bac2de;
    --subtext0: #a6adc8;
    --subtext1: #9399b2;
    --surface: #7f849c;
    --surface0: #6c7086;
    --surface1: #585b70;
    --overlay: #45475a;
    --overlay0: #313244;
    --base: #1e1e2e;
    --crust: #181825;
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
    --sapphire: #89DCEB;
    --sky: #74C7EC;
    --blue: #89B4FA;
    --lavender: #B4BEFE;
}

* {
    box-sizing: border-box;
    margin: 0;
    font-family: 'Inclusive Sans'
}

body {
    color: var(--overlay0);
    size: 1.2em;
    background-color: #cdd6f4;
    max-width: 40em;
    margin: auto;
}

.top {
    top: 0;
    left: 0;
    position: sticky;
    background-color: transparent;
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
    font-size: 1rem;
    background-color: white;
    border: 1px solid #000;
    z-index: 9999;
    box-shadow: 10px 10px var(--base);
}

.div-solid {
    border-top:4px solid #B4BEFE;
    padding-top: 1rem;
    padding-bottom: 1rem;
}

.div-dotted {
    border-top:4px dotted #B4BEFE;
    padding-top: 1rem;
    padding-bottom: 1rem;
}

.pink {
    color: var(--pink);
}

.peach {
    color: var(--peach);
}

.blue {
    color: var(--blue);
}

.lavender {
    color: var(--lavender);
}


.about {
    text-align: center;
}

#education,
#location,
#occupation {
    display: inline-block;
    padding: 0 .5em .2em .5em;
}

.message {
    background-color: white;
    border: 1px solid var(--base);
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
<!--->
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
<--->
<body>
    <div class="container">
    <div class="div">
        <div class="div-solid">
        <div class="intro">
            <h2 class="center">hi, i'm <span style="border-bottom: 3px solid var(--lavender);">laurel</span> <span class="lavender"><i class="fa-solid fa-circle-check"></i></span></h2>
        </div>
        </div><!-->
        <div class="about">
            <div id="location" class="small"><i class="fa-solid fa-location-dot"></i> Mohkínstsis, Earth</div>
            <div id="occupation" class="small"><i class="fa-solid fa-briefcase"></i> PSW</div>
            <div id="education" class="small"><i class="fa-solid fa-graduation-cap"></i> School of Peer Support</div>
            <br><br>
            <p></p>
        </div>    
    </div>
    <--->
    <div class="div">
        <div class="div-dotted"></div>
        <p class="center"> still adjusting things around here <i class="fa-regular fa-face-smile-beam"></i></p>
    </div>
</div>
</body>
</html>