<style>
.cover-coverpage {
  min-height: 100vh;
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%) !important;
  position: relative;
}
.cover-coverpage::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    radial-gradient(circle at 20% 80%, rgba(56, 189, 248, 0.15) 0%, transparent 50%),
    radial-gradient(circle at 80% 20%, rgba(168, 85, 247, 0.1) 0%, transparent 50%),
    radial-gradient(circle at 40% 40%, rgba(236, 72, 153, 0.08) 0%, transparent 40%);
  pointer-events: none;
}
.cover-wrapper {
  display: flex;
  align-items: center;
  gap: 80px;
  max-width: 1100px;
  padding: 60px;
  position: relative;
  z-index: 1;
}
.cover-avatar {
  width: 260px;
  height: 260px;
  border-radius: 24px;
  object-fit: cover;
  box-shadow: 0 25px 80px rgba(56, 189, 248, 0.25);
  border: 4px solid rgba(255,255,255,0.15);
  flex-shrink: 0;
  animation: float 6s ease-in-out infinite;
}
@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}
.cover-content {
  color: #fff;
}
.cover-title {
  font-size: 56px;
  font-weight: 800;
  margin: 0 0 20px 0;
  letter-spacing: 3px;
  background: linear-gradient(135deg, #fff 0%, #38bdf8 50%, #a855f7 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  text-shadow: none;
}
.cover-desc {
  font-size: 20px;
  color: rgba(255,255,255,0.8);
  margin-bottom: 32px;
  line-height: 1.7;
  font-weight: 400;
}
.cover-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-bottom: 40px;
}
.cover-tag {
  background: rgba(56, 189, 248, 0.12);
  color: #38bdf8;
  padding: 10px 20px;
  border-radius: 24px;
  font-size: 15px;
  border: 1px solid rgba(56, 189, 248, 0.25);
  transition: all 0.3s ease;
}
.cover-tag:hover {
  background: rgba(56, 189, 248, 0.2);
  transform: translateY(-2px);
}
.cover-enter-btn {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  background: linear-gradient(135deg, #38bdf8, #0ea5e9);
  color: #0f172a;
  padding: 16px 38px;
  border-radius: 30px;
  text-decoration: none;
  font-size: 17px;
  font-weight: 600;
  transition: all 0.3s ease;
  box-shadow: 0 8px 30px rgba(56, 189, 248, 0.35);
}
.cover-enter-btn:hover {
  transform: translateY(-4px);
  box-shadow: 0 15px 50px rgba(56, 189, 248, 0.45);
  text-decoration: none;
}
.cover-footer {
  margin-top: 50px;
  font-size: 14px;
  color: rgba(255,255,255,0.5);
}
@media (max-width: 768px) {
  .cover-wrapper {
    flex-direction: column;
    text-align: center;
    gap: 40px;
    padding: 30px;
  }
  .cover-avatar {
    width: 180px;
    height: 180px;
  }
  .cover-title {
    font-size: 36px;
  }
  .cover-desc {
    font-size: 16px;
  }
  .cover-tags {
    justify-content: center;
  }
  .cover-avatar {
    animation: none;
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
      <a class="cover-enter-btn" href="#/README">
        👉 进入博客
      </a>
      <div class="cover-footer">Made with ❤️ by 逸夕</div>
    </div>
  </div>
</div>