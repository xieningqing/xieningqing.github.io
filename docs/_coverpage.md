<style>
.cover-coverpage {
  min-height: 100vh;
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
}
.cover-wrapper {
  display: flex;
  align-items: center;
  gap: 60px;
  max-width: 1000px;
  padding: 40px;
}
.cover-avatar {
  width: 220px;
  height: 220px;
  border-radius: 20px;
  object-fit: cover;
  box-shadow: 0 20px 60px rgba(0,0,0,0.4);
  border: 3px solid rgba(255,255,255,0.1);
  flex-shrink: 0;
}
.cover-content {
  color: white;
}
.cover-title {
  font-size: 52px;
  font-weight: 700;
  margin: 0 0 16px 0;
  letter-spacing: 2px;
  background: linear-gradient(135deg, #fff 0%, #38bdf8 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.cover-desc {
  font-size: 18px;
  opacity: 0.85;
  margin-bottom: 30px;
  line-height: 1.6;
}
.cover-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 36px;
}
.cover-tag {
  background: rgba(56, 189, 248, 0.15);
  color: #38bdf8;
  padding: 8px 16px;
  border-radius: 20px;
  font-size: 14px;
  border: 1px solid rgba(56, 189, 248, 0.3);
}
.cover-enter-btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  background: linear-gradient(135deg, #38bdf8, #0ea5e9);
  color: #0f172a;
  padding: 14px 32px;
  border-radius: 30px;
  text-decoration: none;
  font-size: 16px;
  font-weight: 600;
  transition: all 0.3s ease;
  box-shadow: 0 8px 30px rgba(56, 189, 248, 0.35);
}
.cover-enter-btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 40px rgba(56, 189, 248, 0.45);
}
.cover-footer {
  margin-top: 50px;
  font-size: 14px;
  opacity: 0.5;
}
@media (max-width: 768px) {
  .cover-wrapper {
    flex-direction: column;
    text-align: center;
    gap: 30px;
  }
  .cover-avatar {
    width: 160px;
    height: 160px;
  }
  .cover-title {
    font-size: 36px;
  }
  .cover-tags {
    justify-content: center;
  }
}
</style>

<div class="cover-coverpage">
  <div class="cover-wrapper">
    <img class="cover-avatar" src="/assets/img/Bytecode封面.png" alt="avatar">
    <div class="cover-content">
      <h1 class="cover-title">CodeGuide</h1>
      <p class="cover-desc">程序员编码指南 / 技术笔记</p>
      <div class="cover-tags">
        <span class="cover-tag">🧠 面试八股整理</span>
        <span class="cover-tag">💻 后端开发体系</span>
        <span class="cover-tag">🤖 AI工程实践</span>
        <span class="cover-tag">📚 持续更新中</span>
      </div>
      <a class="cover-enter-btn" href="/README.md">
        👉 进入博客
      </a>
      <div class="cover-footer">Made with ❤️ by 逸夕</div>
    </div>
  </div>
</div>