<template>
  <section class="section loan-section" id="loan">
    <div class="section-container">
      <div class="section-content-left">
        <span class="section-tag">대출</span>
        <h2 class="section-title">
          여러 은행의 조건을<br />
          1분 만에 확인해보세요
        </h2>
        <p class="section-description">
          앉은 자리에서 여러 은행의 한도와 금리를 비교하고<br />
          내게 꼭 맞는 대출을 찾아보세요.<br />
          신용, 비상금, 대환, 주택담보대출 모두 가능해요.
        </p>
      </div>
      <div class="section-image-right">
        <div class="phone-mockup medium"></div>
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

.loan-section {
  background: #f9fafb;

  .section-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
    align-items: center;

    &.reverse {
      direction: rtl;

      > * {
        direction: ltr;
      }
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

  &.medium {
    width: 320px;
    height: 640px;
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

  .section-container {
    grid-template-columns: 1fr !important;
  }
}
</style>
