---
layout: home
title: Home
---

<style>
	:root {
		--bg: #FFF8FA;
		--card: #FFE9F1;
		--accent: #FF9CB1;
		--accent-hover: #ff7f9e;
		--text: #222222;
		--radius: 12px;
		--gap: 1.25rem;
		--max-width: 1100px;
		--font-stack: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
	}

	/* Page-level container */
	.home-hero-wrap {
		background: var(--bg);
		color: var(--text);
		font-family: var(--font-stack);
		padding: 4rem 1.25rem;
		display: flex;
		justify-content: center;
	}

	.home-hero {
		width: 100%;
		max-width: var(--max-width);
		display: grid;
		grid-template-columns: 1fr;
		gap: 1.5rem;
		align-items: center;
	}

	.hero-card {
		background: linear-gradient(180deg, var(--card) 0%, rgba(255,232,241,0.75) 100%);
		border-radius: var(--radius);
		padding: 2rem;
		box-shadow: 0 6px 18px rgba(34,34,34,0.06);
	}

	.hero-title {
		margin: 0 0 0.5rem 0;
		font-size: clamp(1.75rem, 4.2vw, 3rem);
		line-height: 1.05;
		color: var(--text);
	}

	.hero-subtitle {
		margin: 0;
		color: var(--text);
		opacity: 0.95;
		font-size: clamp(1rem, 1.6vw, 1.125rem);
	}

	.cta-row { display:flex; gap: 0.75rem; margin-top: 1.25rem; }

	.btn-soft {
		display:inline-block; padding: .65rem 1rem; border-radius: 999px; text-decoration:none;
		background: var(--accent); color: white; font-weight:600; border: none; transition: transform .12s ease, background .12s ease;
	}

	.btn-soft:hover, .card-link:hover { background: var(--accent-hover); transform: translateY(-3px); }

	/* Projects grid */
	.projects-grid {
		display: grid; gap: var(--gap); grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
	}

	.project-card {
		background: linear-gradient(180deg, rgba(255,255,255,0.7), rgba(255,255,255,0.6)), var(--card);
		border-radius: calc(var(--radius) - 2px);
		padding: 1.25rem; color: var(--text); box-shadow: 0 6px 14px rgba(34,34,34,0.06);
		transition: box-shadow .12s ease, transform .12s ease;
	}

	.project-card:hover { box-shadow: 0 16px 36px rgba(34,34,34,0.10); transform: translateY(-6px); }

	.project-title { margin: 0; font-weight:700; font-size: 1.05rem; }

	@media (min-width: 720px) {
		.home-hero { grid-template-columns: 1fr 420px; align-items:center; }
		.hero-intro { padding-right: 2rem; }
	}

	@media (max-width: 480px) {
		.home-hero-wrap { padding: 2.25rem 0.75rem; }
	}
</style>

<div class="home-hero-wrap">
	<div class="home-hero">
		<div class="hero-card hero-intro">
			<h1 class="hero-title">{{ site.author.name | default: "Your Name" }}</h1>
			<p class="hero-subtitle">Hi — I’m {{ site.author.name | default: "Your Name" }}, a product-focused designer & developer. I build simple, beautiful interfaces and thoughtful experiences that solve real problems.</p>

			<div class="cta-row">
				<a href="#projects" class="btn-soft">View projects</a>
				<a href="/about/" class="card-link" style="display:inline-block;padding:.65rem 1rem;border-radius:999px;background:transparent;border:1px solid rgba(34,34,34,0.06);text-decoration:none;color:var(--text);">About me</a>
			</div>
		</div>

		<aside class="hero-card">
			<strong style="display:block;margin-bottom:.5rem;">Quick highlights</strong>
			<ul style="margin:0;padding:0;list-style:none;display:flex;flex-direction:column;gap:.65rem;color:var(--text);">
				<li style="display:flex;align-items:center;gap:.5rem;"><span style="width:9px;height:9px;background:var(--accent);border-radius:999px;display:inline-block;"></span> Available for freelance and remote work</li>
				<li style="display:flex;align-items:center;gap:.5rem;"><span style="width:9px;height:9px;background:var(--accent);border-radius:999px;display:inline-block;"></span> Focus: UI, interaction design, front-end development</li>
			</ul>
		</aside>
	</div>
</div>

<main id="projects" style="padding:2.25rem 1.25rem;max-width:var(--max-width);margin:0 auto;">
	<h2 style="margin-top:0;margin-bottom:1rem;color:var(--text);font-family:var(--font-stack);">Select projects</h2>

	<p style="color:var(--text);opacity:.9;margin-top:0;margin-bottom:1.25rem;">Below are a few examples — click any to see details (placeholders).</p>

	<div class="projects-grid">
		<article class="project-card">
			<h3 class="project-title">Project One — Placeholder</h3>
		</article>

		<article class="project-card">
			<h3 class="project-title">Project Two — Placeholder</h3>
		</article>

		<article class="project-card">
			<h3 class="project-title">Project Three — Placeholder</h3>
		</article>
	</div>
</main>
