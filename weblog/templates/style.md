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
    --toggle: hsl(54, 30%, 39%);
    --link: 
}

.dark-mode {
    --background: hsl(230, 17%, 14%);
    --text: hsl(56, 100%, 94%);
    --toggle: hsl(241, 32%, 29%);
}

body {
    background-color: var(--background);
    color: var(--text);
}


/* .-------------------. */
/* |     ALIGNMENT     | */
/* '-------------------' */

.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
    top: -9rem;
}

* {
	box-sizing: border-box;
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

p, li {
	line-height: 160%;
}

a:link { color: var(--link); }
a:visited { color: var(--link); }
a:hover { color: var(--link); }
a:active { color: var(--link); }


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

img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 90%;
    margin-top: 1rem;
    margin-bottom: 1rem;
}

/* .------------------. */
/* |     SECTIONS     | */
/* '------------------' */

header, main, footer {
	max-width: 60em;
	margin: 1em auto;
	padding: 0 1em;
}

header {
	margin-top: 4em;
    margin-bottom: 3em;
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
    background-color: var(--text);
    color: var(--background);
	margin-top: 8em;
    padding: 1em;
	font-size: 90%;
	text-align: center;
}

/* .---------------. */
/* |     POSTS     | */
/* '---------------' */

.post-info, .post-tags {
	font-size: 85%;
	color: var(--accent);
	text-align: right;
}

.post-info i:nth-child(2) {
	margin-left: .75em;
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

hr {
	border: 0;
	height: 0.1em;
	background: var(--text);
	margin: 2em 0;
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
	background:  #000;
	color:  #eee;
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

.label{
    width: 2.5em;
    height: 1em;
    border-radius: 30px;
    background: var(--toggle);
    position: absolute;
    cursor: pointer;
}
.label:before{
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
    transform: translateX(1.2em);
}

#checkbox {
    display: none;
}

.ball {
    width: 1em;
    height: 1em;
    background-color: var(--background);
    position: absolute;
    border-radius: 50%;
    margin-top: -0.3px;
    margin-left: 3px;
    cursor: pointer;
    transition: all 250ms ease-in-out;
}