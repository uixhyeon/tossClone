<template>
  <section class="section home-section">
    <div class="section-header">
      <span class="section-tag">홈 · 소비</span>
      <h2 class="section-title">
        내 돈 관리,<br />
        지출부터 일정까지 똑똑하게
      </h2>
    </div>
    <div class="section-content">
      <div class="phone-showcase">
        <div class="phone-item">
          <div class="phone-mockup small"></div>
        </div>
        <div class="phone-item">
          <div class="phone-mockup small"></div>
        </div>
      </div>
      <p class="section-description">
        토스에 계좌와 카드를 연결해 보세요.<br />
        계좌 잔액, 대출·투자 내역은 기본,<br />
        일자별 소비와 수입까지 한 번에 볼 수 있어요.
      </p>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.section {
  padding: 120px 40px;
  max-width: 1200px;
  margin: 0 auto;

  .section-header {
    margin-bottom: 80px;

    &.center {
      text-align: center;
    }
  }

  .section-tag {
    display: inline-block;
    font-size: 18px;
    font-weight: 700;
    color: #3182f6;
    margin-bottom: 24px;
  }

  .section-title {
    font-size: 56px;
    font-weight: 700;
    line-height: 1.3;
    color: #191f28;
    margin-bottom: 24px;
  }

  .section-description {
    font-size: 20px;
    line-height: 1.8;
    color: #4e5968;
  }
}

.home-section {
  background: #f9fafb;

  .phone-showcase {
    display: flex;
    gap: 40px;
    justify-content: center;
    margin-bottom: 60px;
  }
}

.phone-mockup {
  width: 280px;
  height: 560px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 40px;
  box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
  position: relative;

  &.small {
    width: 240px;
    height: 480px;
  }

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

@media (max-width: 768px) {
  .section {
    padding: 80px 20px;

    .section-title {
      font-size: 36px !important;
    }
  }
}
</style>
