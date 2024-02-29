Type: Template
Title: Post Template

<style>
    .home-post {
        display: flex;
        align-content: stretch;
        gap: 0em;
        width: 100%;
    }

    .home-post > div {
        padding: 0.1rem;
    }

    .home-post-header {
        text-align: left;
        padding: 0.5rem;
        flex-grow: 1;
    }

    .home-post-image img {
        flex-shrink: 1;
        padding: 1em;
        align-self: flex-start;
        max-height: 15em;
    }

.home-post-title {
    padding: 0;
}

.home-post-info {
    font-size: 0.9em;
    margin-bottom: 0.5rem;
}

@media only screen and (max-width: 380px) {
  /* For mobile phones: */
  .home-post {
    flex-direction: column;
  }
  .home-post-image {
    margin: auto;
  }
  .home-post-img {
    max-height: 5em;
  }

<div class="home-post">
        <div class="home-post-image">
        <a href="{permalink}"><img src="{image}"></a>
        </div>

<div>
    <div class="home-post-header">
        <div class="home-post-info">
            <i class="fa-solid fa-clock"></i> <a href="{permalink}">{date}</a>
            </div>
        <div class="home-post-title">
            <h1 class="large"><span style="text-transform: lowercase;">{title}</span></h1>
            <p>{description}</p>
        </div>
    </div>
</div>