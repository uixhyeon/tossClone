<template>
  <section class="section investment-section" id="investment">
    <div class="section-container reverse">
      <div class="section-image-left">
        <div class="phone-mockup medium"></div>
      </div>
      <div class="section-content-right">
        <span class="section-tag">투자</span>
        <h2 class="section-title">
          투자,<br />
          모두가 할 수 있도록
        </h2>
        <p class="section-description">
          이해하기 쉬운 용어, 설명이 필요 없는<br />
          직관적인 화면 구성, 송금처럼 쉬운<br />
          구매 경험 그리고 투자 판단에 도움을<br />
          주는 콘텐츠까지
        </p>
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

.investment-section {
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

  .investment-section .section-container {
    grid-template-columns: 1fr !important;
  }
}
</style>
