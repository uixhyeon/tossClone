<template>
  <section class="business-section">
    <div class="business-content">
      <h2>사업도 토스와 함께</h2>
      <p>사업을 시작하셨나요?<br />사업의 시작부터 관리까지 이제 토스와 함께 하세요.</p>
      <button class="btn-secondary">사업자 서비스 알아보기</button>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.business-section {
  background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
  color: white;
  text-align: center;
  padding: 120px 40px;

  .business-content {
    h2 {
      font-size: 48px;
      font-weight: 700;
      margin-bottom: 24px;
    }

    p {
      font-size: 20px;
      line-height: 1.8;
      margin-bottom: 48px;
      opacity: 0.9;
    }

    .btn-secondary {
      color: white;
      border-color: white;

      &:hover {
        background: rgba(255, 255, 255, 0.1);
      }
    }
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
  .business-section {
    padding: 80px 20px;

    .business-content h2 {
      font-size: 36px;
    }
  }
}
</style>
