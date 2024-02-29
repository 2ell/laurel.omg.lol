Type: File
Content-Type: text/css
Title: Stylesheet
Location: /style.css








/* ███████████████████████ */
/* █▌                   ▐█ */
/* █▌     VARIABLES     ▐█ */
/* █▌                   ▐█ */
/* ███████████████████████ */



:root {
    --base:  #FDD6AF;
    --background: #f5eee6;
    --text: rgb(50, 49, 87);
    --accent: #ffe5cc;
    --accent2: #797897;
    --accent3: #acacff;
    --link: #acacff6b;
    --link-hov:  #FDD6AF;
    --color-0: #b1a8b9;
    --color1: #cdfde6;
    --color2: #414055;

    --grid-unit: 1em;
    --heading: 'Lily Script One';
}

.dark-mode {
    --background: rgb(7, 6, 22);
    --text: #f5eee6;
    --subtext: #debc99ff;
    --subtext2: rgb(73, 72, 114);
    --accent: hsl(51, 100%, 93%);
    --accent2: rgb(23, 35, 139);
    --base: rgb(12, 20, 85);
    --base2: rgb(255, 222, 190);
    --link: #2229af6c;
    --nav-link: #acacff;
    --link-hov: #444c83;
    --color1: #42a9b1;
    --color2: rgb(5, 8, 37);
}



/* ██████████████████ */
/* █▌              ▐█ */
/* █▌     BASE     ▐█ */
/* █▌              ▐█ */
/* ██████████████████ */

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

.hide {
    display: none;
}

.shadow {
    text-shadow: 3px 1px 1px #f5eee600, 2px 2px 1px var(--accent3), 4px 2px 1px #f5eee6,
    3px 3px 1px var(--accent3), 5px 3px 1px #f5eee600;
}

/* ████████████████████████ */
/* █▌                    ▐█ */
/* █▌     NAVIGATION     ▐█ */
/* █▌                    ▐█ */
/* ████████████████████████ */

.top {
  position: sticky;
  top:0;
  left: 0;
  margin: 0;
  width: 100%;
  height: 4.5rem;
  background-color: var(--accent2);
  z-index: 10000;
}

.top .weblog-title-sm a {
    font-size: 1em;
    color: var(--text);
    margin-left: 0.5rem;
    margin-top: 2rem;
}

.top #navLinks {
  display: none;
  position: relative;
  padding-top: 2rem;
  max-width: 20%;
  background-color: var(--accent2);
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
    color: var(--accent);
    text-decoration: none;
    cursor: pointer;
}

.top #navLinks ul li a:hover {
    background-color: var(--color2);
    transition: all 0.2s ease-in-out;
}

/* Add a grey background color on mouse-over */
.top #navLinks ul li a:hover {
  transition: all 0.2s ease-in-out;
}

/* Style navigation menu links */
.top a.icon {
    position: absolute;
    left: 1.5rem;
    top: 2rem;
    font-size: 1.2em;
    color: var(--nav-link);
    display: block;
    z-index: 10;
}

.top a.icon:hover, .top a.icon:active {
    color: var(--accent);
}


/* . toggle --------. */

.toggle {
    width: 3rem;
    position: absolute;
    top: 0.8rem;
    right: 0.5rem;
}

.label {
    width: 2rem;
    height: 1rem;
    border-radius: 30px;
    background: var(--accent);
    position: absolute;
    cursor: pointer;
}

.label:before {
    content: '';
    position: absolute;
    display: inline-block;
}

.label:after {
    content: '';
    font-size: 1.5rem;
    position: absolute;
    display: inline-block;
}

#checkbox:checked ~ .ball {
    transform: translateX(1rem);
}

#checkbox {
    display: none;
}

.ball {
    width: 0.7rem;
    height: 0.7rem;
    background-color: var(--accent2);
    position: absolute;
    border-radius: 50%;
    margin-top: 2px;
    margin-left: 3px;
    cursor: pointer;
    transition: all 250ms ease-in-out;
}


/* ████████████████████████ */
/* █▌                    ▐█ */
/* █▌     TYPOGRAPHY     ▐█ */
/* █▌                    ▐█ */
/* ████████████████████████ */



h1, h2, h3, h4, h5, h6 {
	font-family: 'Iosevka Web', monospace;
	margin: 1rem 0;
    font-weight: 500;
}

.heading {
    font-family: var(--heading);
    text-shadow: 3px 1px 1px #f5eee600, 2px 2px 1px var(--accent2), 4px 2px 1px #f5eee6,
    3px 3px 1px var(--accent2), 5px 3px 1px #f5eee600;
}

h1 {
    font-size: 3rem;
}

h2 {
    font-size: 3rem;
}

h3 {
    font-size: 2.8rem;
    color: var(--subtext);
}

h4 {
    font-size: 2.3rem;
}

h5 {
    font-size: 2rem;
}

h6 {
    font-size: 1.5rem;
}

/* . type classes --------. */

    .large {
        font-size: 3em;
    }

    .small {
        font-size: 0.8em;
    }

/* . body type --------. */

    p, li {
        line-height: 1.5rem;
        margin-bottom: 1em;
    }



/* ███████████████████ */
/* █▌               ▐█ */
/* █▌     TITLE     ▐█ */
/* █▌               ▐█ */
/* ███████████████████ */

    .title {
        flex-grow: 0;
        margin-top: 2rem;
        margin-right: 1rem;
    }

    .title p {
        margin-top: 0;
        padding-top: 0;
    }

    .weblog-title {
        text-decoration: none;
        font-family: 'Lily Script One';
        color: var(--text); 
        font-size: 8em;
        margin-bottom: 0;
        padding-bottom: 0;
        text-shadow: 3px 1px 1px #f5eee600, 2px 2px 1px var(--accent2), 4px 2px 1px #f5eee6,
    3px 3px 1px var(--accent2), 5px 3px 1px #f5eee600;
    }

/* ████████████████████ */
/* █▌                ▐█ */
/* █▌     IMAGES     ▐█ */
/* █▌                ▐█ */
/* ████████████████████ */

    .head-img, .dark-mode .head-img {
        opacity: 1;
        margin-left: 1rem;
        max-width: 90%;
    }

    .head-img:hover, .dark-mode .head-img:hover {
        opacity: 1;
    }

/* ██████████████████████ */
/* █▌                  ▐█ */
/* █▌     SECTIONS     ▐█ */
/* █▌                  ▐█ */
/* ██████████████████████ */

header, main {
    max-width: 60em;
    margin: auto;
}

main {
    max-width: 60em;
    margin: auto;
}

header {
	margin-top: 0em;
    margin-bottom: 0em;
}

.head-div {
    margin-top: 2em;
    overflow: visible;
    max-height: 35em;
    margin: auto;
    background-color: var(--base);
    display: flex;
    gap: 1rem;
    padding-bottom: 2rem;
}

footer {
    background: var(--color2);
    color: var(--accent);
    margin-top: 1rem;
    padding: 1em;
	font-size: 90%;
	text-align: center;
    border-top: 1px solid var(--accent);
}

footer a { 
    color: var(--accent);
    font-weight: 700;
    text-decoration: none;
    transition: color .3s;
    transition-property: color;
    transition-duration: 0.3s;
    transition-timing-function: ease;
    transition-delay: 0s;
}

footer a:hover { 
    color: var(--nav-link-hov); 
}

.green {
    color: var(--text);
    background-color: var(--color1);
    min-height: 10em;
    padding: 2rem 2rem;
    text-align: right;
}

.div-2 {
    padding: 2rem 2rem;
    color: var(--text);
}

.section {
        padding: 0.5rem;
        gap: 0.5rem;
        display: flex;
        flex-direction: row;
        max-width: 60em;
        margin: auto;
    }

.box-connect-1 {
    flex: 1;
    }

.box-connect-2 {
    flex: 1;
}


.box-connect ul {
    margin-left: 0.2rem;
}


.statuslol {
        color: var(--accent3);
        background-color: var(--base) !important;
        width: 100%;
        padding: 1rem;
        word-wrap: normal !important;
        word-break: keep-all !important;
        overflow-wrap: normal !important;
    }
    .statuslol_content {
        color: var(--text) !important;
        font-size: 1em;
        padding-top: 1rem;
        padding-bottom: 0.5rem !important;
    }
    .statuslol_time:before {
        color: var(--color2) !important;
        font-size: 0.8em;
        content: 'status updated: '
}
    .statuslol_time a {
        color: var(--color2) !important;
        opacity: 1 !important;
        font-size: 0.8em;
}
    .statuslol_emoji_container {
        font-size: 1.4em !important;
        max-height: 2em !important;
        max-width: 2em !important;
        padding-right: 0.5rem !important;
        padding-left: 0.5rem;
        padding-top: 0.5rem;
        background-color: var(--color1);
        border-radius: 8em;
}

.recent-played {
    background: var(--color1);
    text-align: left;
    padding: 1rem;
    width: 100%;
}

.recent-played-track::before {
    content: 'listening to: '
}

.recent-played-track {
    font-size: 1em;
}
    
.connect {
    list-style: none;
}
/* .---------------. */
/* |     POSTS     | */
/* '---------------' */

.post-header {
    margin: 0rem;
    padding: 1rem;
    margin-bottom: 2rem;
    background-color: var(--base);
}

.pagination {
    text-align: center;
}

 a { 
    color: var(--text);
    text-decoration: underline;
    text-decoration-color: currentcolor;
    text-decoration-thickness: auto;
    text-decoration-color: var(--link);
    text-decoration-skip-ink: none;
    text-decoration-thickness: .4rem;
    text-underline-offset: -.18rem;
    transition: text-decoration .3s;
    transition-property: text-decoration;
    transition-duration: 0.3s;
    transition-timing-function: ease;
    transition-delay: 0s;
}

a:hover { 
    text-decoration-color: var(--link-hov); 
}

.content {
    max-width: 40em;
    margin: auto;
    text-align: justify;
    text-justify: inter-word;
    overflow-wrap: break-word;
    hyphens: manual;
    hyphenate-character: '-';
}

hr {
	border: 0;
	height: 0.04rem;
	background: var(--base);
	margin: 4em 0;
    max-width: 100%;
}

code {
	padding: .2em .3em;
	border: 1px solid var(--accent);
	white-space: pre-wrap;
	word-wrap: break-word; 
}

pre, code {
	font-family: 'MD IO 0.4';
	font-size: 0.9em;
}

pre code {
	background: #000;
	color: #eee;
	display: inline-block;
	padding: 1em;
	white-space: pre-wrap;
	word-wrap: break-word;   
}

table {
	border-collapse: collapse;
}

td, th {
	padding: .75em;
	text-align: left;
	border: 1px solid var(--accent);
}


@media only screen and (max-width: 1080px) {
  /* For mobile phones: */
    body {
        font-size: 1em;
    }
    .weblog-title {
        font-size: 6em;
    }
    p, li {
	    line-height: 1.4em;
    }
    .post {
        flex-direction: column;
        justify-content: center;
        margin-bottom: 0;
        padding-bottom: 0;
        padding-left: 0.5rem;
        padding-right: 0.5rem;
    }
    .section {
        flex-direction: column;
        justify-content: center;
    }
    .content {
        max-width: 30em;
        margin: auto;
    }
    .post-image-sm {
        height: 80%;
        width: 100%;
        display: flex;
    }
    .large {
        font-size: 3em;
    }
    .post-title {
        font-size: 3rem;
    }
    .post-subtitle {
        font-size: 2em;
    }
    #navLinks {
        font-size: 1em;
        margin-top: 0em;
        padding-top: 2em;
    }
}


@media only screen and (max-width: 540px) {
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
    .head-img {
        max-width: 15em;
        flex-shrink: 1;
        height: auto;
        margin: auto;
    }
    .title {
        margin-top: -10em;
        margin-left: 1rem;
        margin-bottom: 1rem;
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
    .status {
        margin: 0.5rem;
    }
}







.post {
  display: flex;
  align-content: stretch;
  gap: 1em;
  margin-bottom: 1rem;
}

.post > div {
  padding: 0.2rem;
}

.post-header {
    text-align: left;
    flex-grow: 4;
}

.post-image {
    flex-shrink: 3;
    height: 20em;
    width: 100%;
    margin: auto;
    background-image: url('{image}');
    background-size: cover;
    background-position: center;
}

.post-title {
    padding: 0;
}

.post-info {
    font-size: 0.9em;
    margin-bottom: 0.5rem;
}

.post-tags {
	font-size: 75%;
	color: var(--accent);
    margin-top: 2em;
}

.tag {
	background: var(--accent);
	color: var(--background) !important;
	padding: .3em .4em;
	margin: .8em 0 0 .4em;
	border-radius: .5em;
	text-decoration: none;
	display: inline-block;
}