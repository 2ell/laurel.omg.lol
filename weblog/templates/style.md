Type: File
Content-Type: text/css
Title: Stylesheet
Location: /style.css




/* .-------------------. */
/* |     VARIABLES     | */
/* '-------------------' */


 :root {
    --grid-unit: 1em;
    --background: hsl(56, 100%, 94%);
    --text: hsl(230, 17%, 14%);
    --accent: hsl(54, 30%, 39%);
    --link: hsl(54, 47%, 76%); 
    --link-hov: hsl(54, 30%, 39%);
}

.dark-mode {
    --background: hsl(230, 17%, 14%);
    --text: hsl(56, 100%, 94%);
    --accent: hsl(241, 26%, 51%);
    --link: hsl(242, 53%, 74%);
    --link-hov: hsl(241, 26%, 51%);
}

/* .-------------------. */
/* |        BASE       | */
/* '-------------------' */

* {
	box-sizing: border-box;
}

.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
    top: -9rem;
}

body {
	font-family: 'Lato', sans-serif;
	font-size: 120%;
	color: var(--text);
	background: var(--background);
}


/* .--------------. */
/* |     TEXT     | */
/* '--------------' */

h1, h2, h3, h4, h5, h6 {
	font-family: 'VC Honey Deck', serif;
	margin: 1rem 0;
}

h1 {
    font-size: 200%;
}

p, li {
	line-height: 160%;
}

header a:link { 
    color: var(--text);
    font-weight: 100;
    text-decoration: none;
    transition: color .3s;
    transition-property: color;
    transition-duration: 0.3s;
    transition-timing-function: ease;
    transition-delay: 0s;
}

header a:hover { 
    color: var(--link-hov); 
}

header a:active, header a:visited { 
    color: var(--text); 
}


/* .------------------. */
/* |     HEADINGS     | */
/* '------------------' */

.weblog-title a {
	text-decoration: none;
	color: var(--text);
}

/* .----------------. */
/* |     IMAGES     | */
/* '----------------' */

/* .------------------. */
/* |     SECTIONS     | */
/* '------------------' */

header, main, footer {
	padding: 0 1em;
}

.content {
    max-width: 60em;
    margin: auto;
    min-height: 60vh;
}

header {
	margin-top: 4em;
    margin-bottom: 5em;
}

    header nav ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
    }

    header nav li {
        display: inline-block;
    }

    header nav li a {
        display: block;
        text-decoration: none;
        margin-right: 1em;
    }

footer {
    color: var(--text);
	margin-top: 8em;
    padding: 1em;
	font-size: 90%;
	text-align: center;
    border-top: 1px solid var(--text);
}

footer a:link { 
    color: var(--text);
    font-weight: 100;
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

footer a:active, footer a:visited { 
    color: var(--text); 
}

/* .---------------. */
/* |     POSTS     | */
/* '---------------' */


main a:link { 
    color: var(--text);
    text-decoration: underline;
    /*text-decoration-color: currentcolor;
    text-decoration-thickness: auto;*/
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

main a:active, main a:visited { 
    color: var(--text); 
}

/*
.post-header {
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  flex-direction: row;
  gap: 1em;
  width: 100%;
}
*/
.post-image-th {
    display: block;
  float: left;
  margin-bottom: 2%;
  margin-right: 2%;
  max-width: 25%;
}

.post-image-th img {
  max-width: 100%;
}

.post-image {
  display: block;
  float: left;
  margin-bottom: 2%;
  margin-right: 2%;
  max-width: 50%;
}
    .post-image img {
        max-width: 100%;
    }

.post-title {
    padding-top: 0.8em;
    line-height: 1.2em;
}

.post-info {
	font-size: 75%;
	color: var(--text);
    padding: 0;
    margin: 0;
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

.recent a {
    color: var(text);
    text-decoration: none;
}

.recent a:hover {
    color: var(--link);
}

hr {
	border: 0;
	height: 0.06rem;
	background: var(--text);
	margin: 4em 0;
}

code {
	padding: .2em .3em;
	border: 1px solid var(--accent);
	white-space: pre-wrap;
	word-wrap: break-word; 
}

pre, code {
	font-family: 'MD IO 0.4';
	font-size: 90%;
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


@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  body {
    font-size: 100%;
  }
  .content {
    max-width: 100%;
  }
  .post-header {
    flex-direction: column;
    gap: 0;
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


/* .----------------. */
/* |     TOGGLE     | */
/* '----------------' */


.toggle {
    width: 3%;
    top: 1rem;
    right: 4rem;
    position: absolute;
    margin-bottom: 1rem;
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

.large {
    font-size: 300%;
}