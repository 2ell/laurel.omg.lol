Type: Template
Title: Post Template

<style>
    .home-post {
        display: flex;
        align-content: stretch;
        gap: 1em;
        width: 100%;
    }

    .home-post > div {
        padding: 0.2rem;
    }

    .home-post-header {
        text-align: left;
        padding: 1rem;
        flex-grow: 1;
    }

    .home-post-image {
        flex-shrink: 1;
        padding: 1em;
        align-self: center;
        height: 10em;
        width: 22em;
        background-image: url('{image}');
        background-size: cover;
        background-position: center;
}

.home-post-title {
    padding: 0;
}

.home-post-info {
    font-size: 0.9em;
    margin-bottom: 0.5rem;
}

@media only screen and (max-width: 580px) {
  /* For mobile phones: */
  .home-post {
    flex-direction: column;
  }
  .home-post-image {
    height: 10em;
    width: 20em;
    margin: auto;
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
            <h1 class="large"><span style="text-transform: lowercase;">{title}</span></h1>
            <p>{description}</p>
            </div>
            </div>
            </div>
            </div>
</div>