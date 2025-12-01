
---
layout: page
title: Projects
---

<style>
	:root {
		--bg: #FFF8FA;
		--card: #FFE9F1;
		--accent: #FF9CB1;
		--accent-hover: #ff7f9e;
		--text: #222222;
		--radius: 12px;
		--font-stack: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
		--gap: 1rem;
		--content-max: 1100px;
	}

	.projects-wrap { background: var(--bg); padding: 2.25rem 1rem; font-family: var(--font-stack); color: var(--text); }
	.projects-inner { max-width: var(--content-max); margin: 0 auto; }

	.grid { display:grid; gap:var(--gap); grid-template-columns: 1fr; }

	.card { background: var(--card); border-radius: var(--radius); overflow: hidden; box-shadow: 0 10px 30px rgba(34,34,34,0.06); transition: transform .12s ease, box-shadow .12s ease; }
	.card:hover { transform: translateY(-6px); box-shadow: 0 24px 60px rgba(34,34,34,0.10); }

	.card-figure { height:160px; background: linear-gradient(135deg,var(--accent), rgba(255,255,255,0.6)); display:flex;align-items:center;justify-content:center;color:white;font-weight:700; }
	.card-body { padding: 1rem; }

	.project-title { margin:0;font-size:1.05rem;font-weight:700;color:var(--text); }
	.project-desc { margin:0.5rem 0 0;color:var(--text);opacity:0.9; }

	/* Responsive: 1 / 2 / 3 columns */
	@media (min-width: 620px) { .grid { grid-template-columns: repeat(2, 1fr); } }
	@media (min-width: 980px) { .grid { grid-template-columns: repeat(3, 1fr); } }

	@media (max-width: 480px) { .projects-wrap { padding: 1.25rem .75rem; } }
</style>

<section class="projects-wrap">
	<div class="projects-inner">
		<header style="margin-bottom:1rem;">
			<h1 style="margin:0;">Projects</h1>
			<p style="margin:.5rem 0 1.25rem;color:var(--text);opacity:.9;">A small selection of work — placeholders for now. Tap / click any card to open a project detail page (optional).</p>
		</header>

		<div class="grid">

			<!-- Project 1 -->
			<article class="card">
				<div class="card-figure">Project One — Image</div>
				<div class="card-body">
					<h3 class="project-title">Project One</h3>
					<p class="project-desc">Short description placeholder that summarises the project's goal and impact in one sentence.</p>
				</div>
			</article>

			<!-- Project 2 -->
			<article class="card">
				<div class="card-figure">Project Two — Image</div>
				<div class="card-body">
					<h3 class="project-title">Project Two</h3>
					<p class="project-desc">Short description placeholder that summarises the project's goal and impact in one sentence.</p>
				</div>
			</article>

			<!-- Project 3 -->
			<article class="card">
				<div class="card-figure">Project Three — Image</div>
				<div class="card-body">
					<h3 class="project-title">Project Three</h3>
					<p class="project-desc">Short description placeholder that summarises the project's goal and impact in one sentence.</p>
				</div>
			</article>

		</div>
	</div>
</section>

