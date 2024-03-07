Type: Template
Title: Post Template
<style>

.home-post {
    display: flex;
    background-color: var(--background-alt);
    border-left: 4px solid {color};
    align-items: stretch;
    gap: 0;
    padding: 1rem;
    margin: 1rem;
}

.home-post > div {
    padding: 0.1rem;
}

.home-post-header {
    padding: 0.5rem;
    flex-grow: 1;
}

.home-post-image img {
    flex-shrink: 1;
    padding: 0em;
    align-self: flex-start;
    max-width: 15em;
}

.home-post-title {
    padding: 1rem;
    color: {color};
    text-align: left;
}

.home-post-info {
    font-size: 0.8em;
    margin-top: 1rem;
    margin-bottom: 0.5rem;
    text-align: right;
}

.home-tag::before {
    font-family: 'Font Awesome 5 Free';
    content: '\{fa} ';
    margin-right: .2rem;
    padding-left: .5rem;
}

.home-tag {
    display: block;
    margin-bottom: 1rem;
    font-size: 0.8rem;
    color: {color};
    border-radius: 10px;
    max-width: fit-content;
    padding: .2rem;
}

@media only screen and (max-width: 480px) {
    /* For mobile phones: */
    .home-post {
        flex-direction: column;
        align-items: normal;
    }
    .home-post-title {
        padding: 0;
    }
    .home-post-image {
        padding: 0.5rem;
        margin: auto;
    }
    .home-post-image img {
        max-width: 100%;
        margin: auto;
    }
}
</style>
<div class="home-post">
    <div class="home-post-image">
        <span class="home-tag">tag</span>
    <a href="{permalink}"><img src={image}></a>
    </div>

<div class="home-post-header">
<div class="home-post-info">
        <i class="fa-solid fa-clock"></i> <a href="{permalink}">{date}</a>
    <div class="home-post-title">
        <h1><span style="text-transform: lowercase;">{title}</span></h1>
        <p>{description}</p>
        </div>
    </div>
</div>
</div>