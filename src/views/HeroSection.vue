<template>
  <section class="hero">
    <div class="hero-content">
      <h1 class="hero-title">
        금융의 모든 것<br />
        토스에서 쉽고 간편하게
      </h1>
      <p class="hero-description">
        내 모든 금융 내역을 한눈에 조회하고 한 곳에서 관리하세요.<br />
        이제껏 경험 못 했던 쉽고 편리한 금융 서비스,<br />
        토스와 함께라면 당신의 일상이 새로워질 거예요.
      </p>
      <div class="hero-buttons">
        <button class="btn-primary">앱 다운로드</button>
        <button class="btn-secondary">더 알아보기</button>
      </div>
    </div>
    <div class="hero-image">
      <div class="phone-mockup">
        <div class="phone-screen"></div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.hero {
  padding: 160px 40px 120px;
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: center;

  .hero-content {
    .hero-title {
      font-size: 64px;
      font-weight: 700;
      line-height: 1.2;
      margin-bottom: 32px;
      color: #191f28;
    }

    .hero-description {
      font-size: 20px;
      line-height: 1.6;
      color: #4e5968;
      margin-bottom: 48px;
    }

    .hero-buttons {
      display: flex;
      gap: 16px;
    }
  }

  .hero-image {
    display: flex;
    justify-content: center;
  }
}

.phone-mockup {
  width: 280px;
  height: 560px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 40px;
  box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
  position: relative;

  .phone-screen {
    position: absolute;
    top: 12px;
    left: 12px;
    right: 12px;
    bottom: 12px;
    background: white;
    border-radius: 32px;
  }
}

.btn-primary {
  background: #3182f6;
  color: white;
  border: none;
  padding: 18px 36px;
  font-size: 18px;
  font-weight: 700;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.3s;

  &:hover {
    background: #1b64da;
    transform: translateY(-2px);
    box-shadow: 0 10px 30px rgba(49, 130, 246, 0.3);
  }
}

.btn-secondary {
  background: white;
  color: #3182f6;
  border: 2px solid #3182f6;
  padding: 18px 36px;
  font-size: 18px;
  font-weight: 700;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.3s;

  &:hover {
    background: #f0f7ff;
    transform: translateY(-2px);
  }
}

@media (max-width: 768px) {
  .hero {
    grid-template-columns: 1fr;
    padding: 120px 20px 60px;

    .hero-title {
      font-size: 40px !important;
    }

    .hero-description {
      font-size: 16px !important;
    }
  }
}
</style>
