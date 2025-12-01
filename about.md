
---
layout: page
title: About
---
 My hobbies are watching films with my family, walking, taking pictures for memories, coding and sleeping.
<style>
	:root {
		--bg: #FFF8FA;
		--card: #FFE9F1;
		--accent: #FF9CB1;
		--accent-hover: #ff7f9e;
		--text: #222222;
		--radius: 12px;
		--font-stack: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
		--content-max: 1100px;
	}

	.about-wrap { background: var(--bg); padding: 2.75rem 1rem; font-family: var(--font-stack); color: var(--text); }
	.about-inner { max-width: var(--content-max); margin: 0 auto; display: grid; gap: 1.25rem; grid-template-columns: 1fr; }

	.about-card { background: var(--card); border-radius: var(--radius); padding: 1.25rem; box-shadow: 0 8px 20px rgba(34,34,34,0.06); }

	.about-grid { display:grid; gap:1rem; grid-template-columns: 1fr; align-items: start; }
	.headshot { width:100%; max-width:180px; height:180px; border-radius:999px; background: linear-gradient(135deg,var(--accent), rgba(255,255,255,0.6)); display:block; margin:0 auto; box-shadow: 0 8px 18px rgba(34,34,34,0.06); }

	.bio { padding: .5rem 0; }
	.bio p { margin:.5rem 0; line-height:1.5; }

	.skills { display:flex; flex-wrap:wrap; gap:.5rem; margin-top:.75rem; }
	.skill { padding:.45rem .65rem; border-radius: 999px; background: rgba(255,255,255,0.6); border:1px solid rgba(34,34,34,0.05); font-weight:600; color:var(--text); transition: background .12s ease, transform .12s ease; }
	.skill:hover { background: var(--accent); color: white; transform: translateY(-3px); }

	@media(min-width: 720px){
		.about-inner { grid-template-columns: 1fr; }
		.about-grid { grid-template-columns: 260px 1fr; align-items:center; }
		.headshot { margin:0; }
	}

	@media(max-width: 480px){ .about-wrap { padding: 1.5rem .75rem; } }
</style>

<section class="about-wrap">
	<div class="about-inner">
		<header>
			<h1 style="margin-top:0;">About</h1>
			<p style="margin-top:0;margin-bottom:1rem;color:var(--text);opacity:.9;">A short introduction and highlights about me.</p>
		</header>

		<div class="about-card about-grid">
			<div style="display:flex;align-items:center;justify-content:center;padding:1rem;">
				<!-- Headshot placeholder -->
				<div class="headshot" aria-hidden="true"></div>
			</div>

			<div class="bio">
				<p>Hello — I’m {{ site.author.name | default: "Aida Baghirzade" }}, a designer & front-end developer who cares about clear interfaces, usable interactions, and delightful detail. I take product problems and turn them into practical, modern solutions using clean code and thoughtful visual design.</p>

				<p>My approach blends design thinking with pragmatic engineering — I prototype fast, iterate often, and ship polished projects that focus on user needs and accessibility.</p>

				<div>
					<strong>Core skills</strong>
					<div class="skills">
						<span class="skill">HTML &amp; CSS</span>
						<span class="skill">JavaScript</span>
						<span class="skill">React / Vue</span>
						<span class="skill">UI &amp; Interaction Design</span>
						<span class="skill">Accessibility</span>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

