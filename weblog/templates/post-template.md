Type: Template
Title: Post Template

<style>
    .post-image-th {
    float: left;
    height: 200px;
    width: 200px;
    background-image: url('{image}');
    background-size: cover;
    background-position: top center;
    margin-right: 2em;
    margin-bottom: 2em;
    border: 1px solid var(--text);
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
		