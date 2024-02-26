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
    --text: #333246ff;
    --accent2: #797897;
    --accent: #ffe5cc;
    --link: #ffe5cc;
    --link-hov:  #FDD6AF;
    --nav-link: #ffe5cc;
    --nav-link-hov: #b1a8b9;
    --color1: #6b9e85;
    --color2: #695783;

    --grid-unit: 1em;
    --heading: 'Lily Script One';
}

.dark-mode {
    --background: #333246ff;
    --text: #f5eee6;
    --subtext: #debc99ff;
    --subtext2: rgb(73, 72, 114);
    --accent: rgb(112, 109, 175);
    --accent2: #debc99ff;
    --base: #48465a;
    --base2: #ead4beff;
    --link: #c9ada744;
    --nav-link: #22223b;
    --link-hov: #444c83;
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

/* ████████████████████████ */
/* █▌                    ▐█ */
/* █▌     NAVIGATION     ▐█ */
/* █▌                    ▐█ */
/* ████████████████████████ */

.top {
    top: 0;
    left: 0;
    width: 100%;
    padding: 0.5em;
    padding-bottom: 0;
    margin: 0;
    position: sticky;
    background-color: var(--accent2);
    display: flex;
    z-index: 1000;
    max-height: fit-content;
}

/* . nav links --------. */

.nav {
    text-align: right;
    flex-grow: 1;
}

    .nav .weblog-title-sm a {
        font-family: var(--heading);
        font-size: 1.5em;
        color: var(--accent);
        margin-right: 0.5rem;
    }

    .nav a { 
        color: var(--nav-link);
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
                margin: 0em;
                margin-right: 0.5rem;
                padding: 0em;
            }

            .nav li {
                display: inline-block;
            }

            .nav li a {
                display: block;
                text-decoration: none;
                margin-left: 1em;
            }


/* . toggle --------. */

.toggle {
    width: 3%;
    top: 0.3rem;
    left: 0rem;
    position: relative;
    margin-bottom: 1rem;
    flex-shrink: 1;
}

.label {
    width: 2.5rem;
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
    transform: translateX(1.4em);
}

#checkbox {
    display: none;
}

.ball {
    width: 0.8rem;
    height: 0.8rem;
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
}

h1 {
    font-size: 4rem;
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
    }

/* ████████████████████ */
/* █▌                ▐█ */
/* █▌     IMAGES     ▐█ */
/* █▌                ▐█ */
/* ████████████████████ */

    .head-img, .dark-mode .head-img {
        opacity: 1;
        margin-left: 1rem;
        max-width: 80%;
    }

    .head-img:hover, .dark-mode .head-img:hover {
        opacity: 1;
    }

    .post-image-sm {
        display: none;
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
    background-color: var(--base);
    display: flex;
    padding-bottom: 2rem;
}

footer {
    background: var(--accent2);
    color: var(--accent);
    margin-top: 1rem;
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

.div-1 {
    color: var(--accent);
    background-color: var(--color1);
    min-height: 10em;
    padding: 2rem 2rem;
    text-align: right;
}

.div-2 {
    padding: 2rem 2rem;
    color: var(--text);
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

main a { 
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
    max-width: 30em;
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
        padding-right: 1rem;
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
    .nav {
        font-size: 1em;
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
    .weblog-title {
        text-align: center;
        color: var(--background);
        margin-left: 0em;
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