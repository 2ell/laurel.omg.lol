Type: Template
Title: Post Template

<style>
    .post {
        display: flex;
        align-content: stretch;
        gap: 1em;
        background-color: var(--accent);
    }

    .post > div {
        background-color: #00f;
    }

    .post-header {
        text-align: left;
        width: 100%;
        flex-grow: 4;
    }

    .post-image-th {
        flex-shrink: 2;
        height: 10em;
        width: 20em;
        background-image: url('{image}');
        background-size: cover;
        background-position: center;
        border: 1px solid #000;
}

.post-title {
    padding: 0;
}

.post-info {
    font-size: 0.9em;
    margin-bottom: 0.5rem;
}
</style>


<article>

<div class="post">
        <div class="post-image">
        </div>

<div>
    <div class="post-header">
        <div class="post-info">
            <i class="fa-solid fa-clock"></i> <a href="{permalink}">{date}</a>
        <div class="post-title">
            <h1 class="large">{title}</h1>
            </div>
            </div>
            </div>
            </div>
</div>
<p>{description}</p>
		