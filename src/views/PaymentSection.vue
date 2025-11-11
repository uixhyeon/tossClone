<template>
  <section class="section payment-section" id="payment">
    <div class="section-header center">
      <span class="section-tag">결제</span>
      <h2 class="section-title">
        결제는 간편하게,<br />
        할인과 적립은 두둑히
      </h2>
    </div>

    <div class="payment-showcase">
      <div class="payment-item">
        <div class="phone-mockup small"></div>
        <p>온라인과 오프라인 모두<br />토스로 간편하게 결제해요.</p>
      </div>
      <div class="payment-item">
        <div class="phone-mockup small"></div>
        <p>쿠폰과 포인트로 할인 받고<br />토스프라임 적립까지 받아요.</p>
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

.payment-showcase {
  display: flex;
  gap: 60px;
  justify-content: center;

  .payment-item {
    text-align: center;

    p {
      margin-top: 32px;
      font-size: 20px;
      line-height: 1.6;
      color: #4e5968;
    }
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

  .payment-showcase {
    flex-direction: column;
  }
}
</style>
