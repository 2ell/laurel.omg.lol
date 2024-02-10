Type: Template
Title: Post Template

<style>
    .home-post {
        display: flex;
        align-content: stretch;
        gap: 1em;
        background-color: var(--accent);
        width: 100%;
    }

    .home-post > div {
        padding: 0.2rem;
    }

    .home-post-header {
        text-align: left;
        width: 100%;
        flex-grow: 4;
    }

    .home-post-image {
        flex-shrink: 2;
        height: 10em;
        width: 20em;
        background-image: url('{image}');
        background-size: cover;
        background-position: center;
        border: 1px solid #000;
}

.home-post-title {
    padding: 0;
}

.home-post-info {
    font-size: 0.9em;
    margin-bottom: 0.5rem;
}
</style>

<div class="home-post">
        <div class="home-post-image">
        </div>

<div>
    <div class="home-post-header">
        <div class="home-post-info">
            <i class="fa-solid fa-clock"></i> <a href="{permalink}">{date}</a>
        <div class="home-post-title">
            <h1 class="large">{title}</h1>
            </div>
            </div>
            </div>
            </div>
</div>
<p>{description}</p>