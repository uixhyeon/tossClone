<template>
  <section class="section convenience-section">
    <div class="section-header center">
      <h2 class="section-title">
        금융을 넘어<br />
        일상을 더 편리하게
      </h2>
    </div>

    <div class="convenience-grid">
      <div class="convenience-card large">
        <div class="card-content">
          <h3>세금 납부, 등본 발급까지<br />토스로 한 번에</h3>
          <p>놓치기 쉬운 세금 납부 및 환급은 물론<br />주민등록 등초본까지 편하게 신청하세요.</p>
        </div>
      </div>

      <div class="convenience-card">
        <div class="card-content">
          <span class="card-tag">보험</span>
          <h3>조회부터 상담,<br />병원비 돌려받기를<br />간편하게</h3>
          <p>전문가 상담을 통해 내게 딱 맞는<br />보험을 추천받으세요.</p>
        </div>
      </div>

      <div class="convenience-card">
        <div class="card-content">
          <span class="card-tag">부동산 · 자동차</span>
          <h3>내 부동산 · 자동차<br />정기적으로 관리해보세요</h3>
          <p>시세조회부터 관리비 납부,<br />보험료 조회까지 한 번에.</p>
        </div>
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

.convenience-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 24px;

  .convenience-card {
    background: #f9fafb;
    padding: 60px 48px;
    border-radius: 32px;
    transition: all 0.3s;

    &:hover {
      transform: translateY(-8px);
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.12);
    }

    &.large {
      grid-column: span 2;
      background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
      color: white;

      h3,
      p {
        color: white;
      }
    }

    .card-tag {
      display: inline-block;
      font-size: 16px;
      font-weight: 700;
      color: #3182f6;
      margin-bottom: 16px;
    }

    h3 {
      font-size: 32px;
      font-weight: 700;
      margin-bottom: 20px;
      line-height: 1.3;
    }

    p {
      font-size: 18px;
      line-height: 1.6;
      color: #6b7684;
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

  .convenience-grid {
    grid-template-columns: 1fr !important;
  }
}
</style>
