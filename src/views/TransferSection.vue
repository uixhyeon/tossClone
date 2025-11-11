<template>
  <section class="section transfer-section" id="transfer">
    <div class="section-header">
      <span class="section-tag">송금</span>
      <h2 class="section-title">
        간편하고 안전하게<br />
        수수료는 평생 무료로
      </h2>
    </div>

    <div class="feature-grid">
      <div class="feature-card highlight">
        <div class="feature-icon">💸</div>
        <h3>평생 무료 송금</h3>
        <p>누구에게 보내든 은행 상관 없이,<br />수수료 걱정 없이 송금하세요.</p>
      </div>

      <div class="feature-card">
        <div class="feature-icon">🛡️</div>
        <h3>사기계좌 조회</h3>
        <p>송금 전 토스가 알아서<br />사기 내역을 조회해드려요.</p>
      </div>

      <div class="feature-card">
        <div class="feature-icon">⏰</div>
        <h3>자동이체 예약</h3>
        <p>은행 점검 시간이 끝나면<br />토스가 알아서 송금해드릴게요.</p>
      </div>
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

.feature-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;

  .feature-card {
    background: #f9fafb;
    padding: 48px 36px;
    border-radius: 24px;
    transition: all 0.3s;

    &:hover {
      transform: translateY(-8px);
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    }

    &.highlight {
      grid-column: span 2;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;

      h3,
      p {
        color: white;
      }
    }

    .feature-icon {
      font-size: 48px;
      margin-bottom: 24px;
    }

    h3 {
      font-size: 28px;
      font-weight: 700;
      margin-bottom: 16px;
      color: #191f28;
    }

    p {
      font-size: 18px;
      line-height: 1.6;
      color: #4e5968;
    }
  }
}

@media (max-width: 768px) {
  .section {
    padding: 80px 20px;

    .section-title {
      font-size: 36px !important;
    }
  }

  .feature-grid,
  .credit-grid,
  .convenience-grid {
    grid-template-columns: 1fr !important;
  }

  .feature-card.highlight {
    grid-column: span 1 !important;
  }
}
</style>
