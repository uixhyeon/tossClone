<template>
  <section class="section credit-section" id="credit">
    <div class="section-header center">
      <span class="section-tag">신용</span>
      <h2 class="section-title">
        금융 생활의 첫 걸음,<br />
        신용점수를 미리 무료로 관리하세요
      </h2>
    </div>

    <div class="credit-grid">
      <div class="credit-card">
        <div class="credit-icon">📊</div>
        <h3>내 신용점수</h3>
        <p>언제 어디서든 KCB, NICE 신용점수를<br />한 곳에서 확인할 수 있어요.</p>
      </div>

      <div class="credit-card">
        <div class="credit-icon">📈</div>
        <h3>신용점수 올리기</h3>
        <p>통신비, 납부내역 등의 서류를<br />토스에서 바로 제출해 점수를 올려요.</p>
      </div>

      <div class="credit-card">
        <div class="credit-icon">🔔</div>
        <h3>신용관리 알림</h3>
        <p>신용점수에 변동이 생기면<br />토스가 알람을 보내드려요.</p>
      </div>

      <div class="credit-card">
        <div class="credit-icon">💡</div>
        <h3>신용관리 팁</h3>
        <p>신용점수 관리가 막막하다면?<br />신용관리 팁을 읽어보세요.</p>
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

.credit-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 24px;

  .credit-card {
    background: #f9fafb;
    padding: 40px 32px;
    border-radius: 20px;
    text-align: center;
    transition: all 0.3s;

    &:hover {
      transform: translateY(-4px);
      background: white;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    }

    .credit-icon {
      font-size: 56px;
      margin-bottom: 24px;
    }

    h3 {
      font-size: 20px;
      font-weight: 700;
      margin-bottom: 16px;
      color: #191f28;
    }

    p {
      font-size: 16px;
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

  .credit-grid {
    grid-template-columns: 1fr !important;
  }
}
</style>
