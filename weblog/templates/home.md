Type: Template
Title: Landing Page Template

<!DOCTYPE html>
<html lang="en">
<head>
<title>{weblog-title}{separator}</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
{feeds}
<style>
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-lato-regular.css');
@import url('https://static.omg.lol/type/font-lato-bold.css');
@import url('https://static.omg.lol/type/font-lato-italic.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
</style>
<link rel="stylesheet" href="https://laurel.omg.lol/style.css">
</head>
<body>

<header>
	<h1 class="weblog-title"><a href="{base-path}">{weblog-title}</a></h1>
	{navigation}
</header>

<main>

<article>
	{body}
	<aside class="post-info">
		<i class="fa-solid fa-clock"></i> {date}
	</aside>
	<aside class="post-tags">
		{tags}
	</aside>
</article>

<hr>

<h2>Recent posts</h2>

{recent-posts}

</main>

<footer>
	<p>Made with <a href="https://weblog.lol">weblog.lol</a>.</p>
</footer>

</body>
</html>