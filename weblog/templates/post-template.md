Type: Template
Title: Post Template

<style>
    .post-image-th {
    max-height: 50%;
    width: auto;
    background-image: url('{image}');
    background-size: cover;
    background-position: center;
    margin-bottom: 2em;
    border: 1px solid var(--text);
    background-repeat: no-repeat;
}
</style>

<div class="post-info">
    <i class="fa-solid fa-clock"></i> <a href="{permalink}">{date}</a>
</div>
<br>
<article>
        <div class="post-image-th">
    </div>
    <div class="post-title">
    <h1 class="large">{title}</h1>
    </div>
<p>{description}</p>
<br>
</article>
</div>
</div>
		