Type: File
Content-Type: text/css
Title: Stylesheet
Location: /style.css



/* .-------- VARIABLES --------. */


 :root {
    --grid-unit: 1em;
    --background: hsl(227, 68%, 88%);
    --text: hsl(232, 23%, 18%);
    --subtext: hsl(230, 19%, 26%);
    --subtext2: hsl(230, 14%, 41%);
    --accent:hsl(230, 14%, 41%);
    --base: hsl(171, 47%, 69%);
    --link: hsl(233, 23%, 15%);
    --link-hov: hsl(171, 47%, 69%);
}

.dark-mode {
    --background: hsl(232, 23%, 18%);
    --text: hsl(227, 68%, 88%);
    --subtext: hsl(228, 39%, 80%);
    --subtext2: hsl(230, 14%, 41%);
    --accent: hsl(172, 39%, 65%);
    --base: hsl(233, 23%, 15%);
    --link: hsl(230, 14%, 41%);
    --link-hov: hsl(170, 23%, 45%);
}

/* .-------- BASE --------. */

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

/* .-------- NAVIGATION --------. */

.top {
    top: 0;
    left: 0;
    width: 100%;
    padding: 1em;
    margin: 0;
    position: sticky;
    background-color: var(--base);
    display: flex;
    z-index: 1000;
}

/* .-------- nav links --------. */

.nav {
    text-align: right;
    flex-grow: 1;
}

.nav a { 
    color: var(--text);
    font-weight: 300;
    text-decoration: none;
    transition: color .3s ease-in-out;
}

.nav a:hover { 
    color: var(--link-hov); 
    transition: color .3s ease-in-out;
}

.nav ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
    }

    .nav li {
        display: inline-block;
    }

    .nav li a {
        display: block;
        text-decoration: none;
        margin-right: 1em;
    }


/* .-------- toggle --------. */

.toggle {
    width: 3%;
    top: 0.1rem;
    left: 0rem;
    position: relative;
    margin-bottom: 1rem;
    flex-shrink: 1;
}

.label {
    width: 2.5em;
    height: 1em;
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
    transform: translateX(1.4em);
}

#checkbox {
    display: none;
}

.ball {
    width: 0.8em;
    height: 0.8em;
    background-color: var(--background);
    position: absolute;
    border-radius: 50%;
    margin-top: 2px;
    margin-left: 3px;
    cursor: pointer;
    transition: all 250ms ease-in-out;
}

/* .-------- typography --------. */

h1, h2, h3, h4, h5, h6 {
	font-family: 'Iosevka Web', monospace;
	margin: 1rem 0;
    font-weight: 500;
}

h1 {
    font-size: 2rem;
}

h3 {
    color: var(--subtext);
}

.large {
    font-size: 3em;
}

p, li {
	line-height: 1.5rem;
}

/* .------------------. */
/* |     HEADINGS     | */
/* '------------------' */

.weblog-title a {
	text-decoration: none;
	color: var(--text);
    font-weight: 700;
}

.weblog-title a { 
    color: var(--text);
    text-decoration: underline;
    text-decoration-color: currentcolor;
    text-decoration-thickness: auto;
    text-decoration-color: var(--background);
    text-decoration-skip-ink: none;
    text-decoration-thickness: .6rem;
    text-underline-offset: -.12rem;
    transition: text-decoration .3s;
    transition-property: text-decoration;
    transition-duration: 0.3s;
    transition-timing-function: ease;
    transition-delay: 0s;
}
.weblog-title a:hover { 
    text-decoration-color: var(--link-hov); 
}

/* .----------------. */
/* |     IMAGES     | */
/* '----------------' */

/* .------------------. */
/* |     SECTIONS     | */
/* '------------------' */

header, main {
	padding: 0;
    max-width: 60em;
    margin: auto;
}

header {
	margin-top: 0em;
    margin-bottom: 5em;
}

footer {
    color: var(--text);
	margin-top: 8em;
    padding: 1em;
	font-size: 90%;
	text-align: center;
    border-top: 1px solid var(--accent);
}

footer a { 
    color: var(--text);
    font-weight: 700;
    text-decoration: none;
    transition: color .3s;
    transition-property: color;
    transition-duration: 0.3s;
    transition-timing-function: ease;
    transition-delay: 0s;
}

footer a:hover { 
    color: var(--link-hov); 
}

/* .---------------. */
/* |     POSTS     | */
/* '---------------' */

.content {
    max-width: 60em;
    margin: auto;
    padding-left: 1rem;
    text-align: justify;
    text-justify: inter-word;
}

main a { 
    color: var(--text);
    text-decoration: underline;
    text-decoration-color: currentcolor;
    text-decoration-thickness: auto;
    text-decoration-color: var(--link);
    text-decoration-skip-ink: none;
    text-decoration-thickness: .2rem;
    text-underline-offset: -.12rem;
    transition: text-decoration .3s;
    transition-property: text-decoration;
    transition-duration: 0.3s;
    transition-timing-function: ease;
    transition-delay: 0s;
}
main a:hover { 
    text-decoration-color: var(--link-hov); 
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
    flex-shrink: 2;
    height: 200px;
    width: 580px;
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

.recent {
    margin-left: 1rem;
    margin-right: 1rem;
}

.recent a {
    color: var(--text);
    text-decoration: none;
    transition: color .3s ease;
}

.recent a:hover {
    color: var(--link-hov);
    transition: color .3s ease;
}

hr {
	border: 0;
	height: 0.04rem;
	background: var(--accent);
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


@media only screen and (max-width: 580px) {
  /* For mobile phones: */
  body {
    font-size: 1em;
  }
  p, li {
	line-height: 1.2em;
}
    .post {
    flex-direction: column;
    justify-content: center;
    margin-bottom: 0;
    padding-bottom: 0;
}
.content {
    padding-left: 1rem;
    padding-right: 1rem;
    max-width: 100%;
}
    .post-image {
        height: 10em;
        width: 20em;
    }
  .large {
    font-size: 3em;
  }
  .nav {
    font-size: 0.8em;
  }
}

/* .-------------------. */
/* |     DARK MODE     | */
/* '-------------------' */


.dark-mode img {
    opacity: 0.7;
    transition: all 0.4s ease-in-out;
}

.dark-mode img:hover {
    opacity: 1;
    transition: all 0.4s ease-in-out;
}