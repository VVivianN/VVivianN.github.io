<script setup lang="ts">
</script>

<template>
  <div class="page">
    <header class="hero">
      <div class="hero-content">
        <p class="eyebrow">个人网站 · Portfolio</p>
        <h1>你的名字</h1>
        <p class="subtitle">前端工程师 / 设计工程师 / 产品工程师</p>
        <p class="intro">
          我专注于把复杂想法做成清晰、有质感的产品体验。
          这里展示我的项目、技能与联系方式。
        </p>
        <div class="cta">
          <a class="btn primary" href="mailto:you@email.com">联系我</a>
          <a class="btn ghost" href="https://github.com/yourname" target="_blank">GitHub</a>
        </div>
      </div>

      <div class="hero-card">
        <div class="avatar">YN</div>
        <div class="card-meta">
          <div class="role">前端 / 全栈</div>
          <div class="location">中国 · 上海</div>
        </div>
        <div class="tag-row">
          <span class="tag">Vue</span>
          <span class="tag">TypeScript</span>
          <span class="tag">UI/UX</span>
        </div>
      </div>
    </header>

    <section id="about" class="section">
      <h2>关于我</h2>
      <p>
        我擅长从业务目标出发，拆解复杂问题并落地高质量界面与交互。
        对设计细节、性能和可维护性有持续追求。
      </p>
    </section>

    <section id="projects" class="section">
      <h2>项目</h2>
      <div class="grid">
        <article class="card">
          <h3>项目 A</h3>
          <p>一句话描述项目亮点，例如提升转化率或优化流程。</p>
          <div class="card-foot">
            <span>Vue · Vite · Pinia</span>
            <a href="#" target="_blank">查看</a>
          </div>
        </article>
        <article class="card">
          <h3>项目 B</h3>
          <p>一句话描述项目亮点，例如从 0 到 1 构建。</p>
          <div class="card-foot">
            <span>Node · TS · Postgres</span>
            <a href="#" target="_blank">查看</a>
          </div>
        </article>
        <article class="card">
          <h3>项目 C</h3>
          <p>一句话描述项目亮点，例如性能提升 40%。</p>
          <div class="card-foot">
            <span>SSR · SEO · CI/CD</span>
            <a href="#" target="_blank">查看</a>
          </div>
        </article>
      </div>
    </section>

    <section id="skills" class="section">
      <h2>技能</h2>
      <div class="pill-grid">
        <span class="pill">HTML/CSS</span>
        <span class="pill">Vue / React</span>
        <span class="pill">TypeScript</span>
        <span class="pill">Node.js</span>
        <span class="pill">Figma</span>
        <span class="pill">性能优化</span>
      </div>
    </section>

    <section id="contact" class="section contact">
      <h2>联系</h2>
      <p>如果你想合作或聊聊项目，欢迎联系我。</p>
      <div class="cta">
        <a class="btn primary" href="mailto:you@email.com">发送邮件</a>
        <a class="btn ghost" href="https://www.linkedin.com/in/yourname" target="_blank">LinkedIn</a>
      </div>
    </section>

    <footer class="footer">
      <span>? 2026 你的名字</span>
      <span>Built with Vue + Vite</span>
    </footer>
  </div>
</template>

<style scoped>
:global(body) {
  margin: 0;
  background: radial-gradient(1200px 600px at 10% 10%, #fff1c1 0%, transparent 60%),
              radial-gradient(1000px 800px at 90% 20%, #c2e8ff 0%, transparent 55%),
              #f7f6f2;
  color: #1d1d1f;
  font-family: "Space Grotesk", "Noto Sans SC", sans-serif;
}

.page {
  max-width: 1100px;
  margin: 0 auto;
  padding: 48px 24px 64px;
}

.hero {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 32px;
  align-items: center;
}

.hero-content h1 {
  font-size: 48px;
  line-height: 1.05;
  margin: 8px 0 12px;
}

.eyebrow {
  letter-spacing: 0.2em;
  text-transform: uppercase;
  font-size: 12px;
  color: #6b6b6b;
}

.subtitle {
  font-size: 18px;
  color: #333;
  margin: 0 0 12px;
}

.intro {
  font-size: 16px;
  line-height: 1.6;
  color: #2f2f2f;
}

.cta {
  display: flex;
  gap: 12px;
  margin-top: 20px;
}

.btn {
  padding: 10px 16px;
  border-radius: 999px;
  text-decoration: none;
  font-weight: 600;
  font-size: 14px;
  border: 1px solid #1d1d1f;
}

.btn.primary {
  background: #1d1d1f;
  color: #fff;
}

.btn.ghost {
  background: transparent;
  color: #1d1d1f;
}

.hero-card {
  background: #ffffffcc;
  border: 1px solid #e2e2e2;
  border-radius: 20px;
  padding: 24px;
  backdrop-filter: blur(6px);
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
}

.avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  background: #111;
  color: #fff;
  font-weight: 700;
  display: grid;
  place-items: center;
  margin-bottom: 12px;
}

.card-meta {
  display: flex;
  justify-content: space-between;
  font-size: 14px;
  color: #444;
}

.tag-row {
  margin-top: 12px;
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
}

.tag {
  font-size: 12px;
  padding: 4px 10px;
  border-radius: 999px;
  background: #f0f0f0;
}

.section {
  margin-top: 56px;
}

.section h2 {
  font-size: 24px;
  margin-bottom: 12px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

.card {
  background: #fff;
  border: 1px solid #e6e6e6;
  border-radius: 16px;
  padding: 16px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.06);
}

.card-foot {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 12px;
  font-size: 12px;
}

.pill-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.pill {
  padding: 6px 12px;
  border-radius: 999px;
  background: #fff;
  border: 1px solid #e2e2e2;
  font-size: 13px;
}

.contact {
  background: #ffffffcc;
  border: 1px solid #e2e2e2;
  border-radius: 16px;
  padding: 24px;
  backdrop-filter: blur(4px);
}

.footer {
  display: flex;
  justify-content: space-between;
  margin-top: 56px;
  font-size: 12px;
  color: #666;
}

@media (max-width: 900px) {
  .hero {
    grid-template-columns: 1fr;
  }
  .grid {
    grid-template-columns: 1fr;
  }
}
</style>
