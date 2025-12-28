### Github codes

<style>
.github-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1rem;
  margin-top: 1rem;
}

.github-tile {
  background: #f8f9fa;
  padding: 0.9em;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.08);
  transition: 0.2s ease;
}

.github-tile:hover {
  background: #eef1f4;
  transform: translateY(-2px);
}

.github-link {
  text-decoration: none;
  font-weight: 600;
  color: #0366d6;
  display: flex;
  align-items: center;
  gap: 0.5em;
  margin-bottom: 0.4em;
}

.github-link:hover {
  text-decoration: underline;
}

.github-icon {
  width: 18px;
  height: 18px;
}
</style>

<style>
/* Grid layout */
.github-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.2rem;
  margin-top: 1rem;
}

/* Modern card style */
.github-tile {
  background: #ffffff; /* white background */
  padding: 1em;
  border-radius: 12px; /* smooth rounded edges */
  box-shadow: 0 4px 12px rgba(0,0,0,0.08); /* soft shadow */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  transition: all 0.3s ease;
}

.github-tile:hover {
  transform: translateY(-4px); /* lift effect */
  box-shadow: 0 8px 20px rgba(0,0,0,0.12); /* slightly stronger shadow on hover */
}

/* Project image/logo */
.github-tile img.project-img {
  width: 60px;
  height: 60px;
  object-fit: cover;
  border-radius: 6px;
  margin-bottom: 0.8em;
}

/* GitHub link/title */
.github-tile a.github-link {
  display: flex;
  align-items: center;
  gap: 0.4em;
  font-weight: 700;
  font-size: 1.05em;
  color: #111111; /* very dark text */
  text-decoration: none;
  margin-bottom: 0.4em;
}

.github-tile a.github-link:hover {
  color: #0366d6; /* GitHub blue on hover */
  text-decoration: underline;
}

/* Description text */
.github-tile span {
  font-size: 0.9em;
  color: #333333; /* dark description */
  line-height: 1.4em;
}

/* GitHub icon */
.github-icon {
  width: 18px;
  height: 18px;
}
</style>

<div class="github-grid">

  <!-- IndraEye -->
  <div class="github-tile">
    <a href="https://github.com/airl-iisc/IndraEye" target="_blank" class="github-link">
      <img class="github-icon"
           src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png"
           alt="GitHub">
      IndraEye
    </a>
    <span>A large-scale ophthalmic imaging dataset designed for automated diagnosis and research in medical imaging.</span>
  </div>

  <!-- MRFP -->
  <div class="github-tile">
    <a href="https://github.com/airl-iisc/MRFP" target="_blank" class="github-link">
      <img class="github-icon"
           src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png"
           alt="GitHub">
      MRFP
    </a>
    <span>Multi-robot perception & planning framework for robotics research and development.</span>
  </div>

  <!-- OV-COAST -->
  <div class="github-tile">
    <a href="https://github.com/adityagandhamal/OV-COAST/" target="_blank" class="github-link">
      <img class="github-icon"
           src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png"
           alt="GitHub">
      OV-COAST
    </a>
    <span>Open-source tools for coastal & oceanic sensing, including data collection and analysis frameworks.</span>
  </div>

</div>

