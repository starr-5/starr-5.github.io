
---
layout: page
title: Contact
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
		--content-max: 900px;
	}

	.contact-wrap { background: var(--bg); padding: 2.25rem 1rem; font-family: var(--font-stack); color: var(--text); }
	.contact-inner { max-width: var(--content-max); margin: 0 auto; display:grid; gap:1rem; }

	.contact-card { background: var(--card); border-radius: var(--radius); padding: 1.25rem; box-shadow: 0 10px 30px rgba(34,34,34,0.06); }
	.contact-row { display:flex; gap:1rem; align-items:center; flex-wrap:wrap; }

	.contact-email { display:inline-block; padding:.6rem .9rem; border-radius:999px; background:var(--accent); color:#fff; text-decoration:none; font-weight:700; transition: background .12s ease, transform .12s ease; }
	.contact-email:hover { background:var(--accent-hover); transform: translateY(-3px); }

	.social-links { display:flex; gap:.75rem; align-items:center; flex-wrap:wrap; }
	.social-link { padding:.45rem .75rem; border-radius: 999px; background: rgba(255,255,255,0.6); border:1px solid rgba(34,34,34,0.05); text-decoration:none; color:var(--text); font-weight:600; transition: background .12s ease, transform .12s ease; }
	.social-link:hover { background: var(--accent); color: white; transform: translateY(-3px); }

	@media(max-width: 480px) { .contact-wrap { padding: 1.25rem .75rem; } .contact-row { flex-direction:column; align-items:flex-start; } }
</style>

<section class="contact-wrap">
	<div class="contact-inner">
		<header>
			<h1 style="margin:0;">Contact</h1>
			<p style="margin:.5rem 0 1rem;color:var(--text);opacity:.9;">I’m happy to hear from you — whether it’s a project idea, collaboration, or a quick hello.</p>
		</header>

		<div class="contact-card">
			<div class="contact-row">
				<a class="contact-email" href="mailto:your-email@example.com">your-email@example.com</a>

				<div style="flex:1; display:flex; justify-content:flex-end;">
					<div class="social-links">
						<a class="social-link" href="https://github.com/your-username" target="_blank" rel="noopener">GitHub</a>
						<a class="social-link" href="https://www.codecademy.com/profiles/your-username" target="_blank" rel="noopener">Codecademy</a>
					</div>
				</div>
			</div>
		</div>

		<footer style="font-size:.95rem;color:var(--text);opacity:.8;padding-top: .5rem;">Prefer not to share email? You can also reach me by opening a GitHub issue on a project or via social links above.</footer>
	</div>
</section>

