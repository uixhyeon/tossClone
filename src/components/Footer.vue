<template>
  <footer class="footer">
    <div class="footer-container">
      <div class="footer-logo">toss</div>
      <div class="footer-links">
        <div class="footer-column">
          <h4>서비스</h4>
          <a href="#">공지사항</a>
          <a href="#">자주 묻는 질문</a>
          <a href="#">공동인증서 관리</a>
        </div>
        <div class="footer-column">
          <h4>회사</h4>
          <a href="#">회사 소개</a>
          <a href="#">채용</a>
          <a href="#">팀 블로그</a>
        </div>
        <div class="footer-column">
          <h4>문의</h4>
          <a href="#">전화: 1599-4905</a>
          <a href="#">이메일: support@toss.im</a>
        </div>
      </div>
      <div class="footer-bottom">
        <p>© 2025 Toss Clone. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  background: #f9fafb;
  padding: 80px 40px 40px;

  .footer-container {
    max-width: 1200px;
    margin: 0 auto;
  }

  .footer-logo {
    font-size: 32px;
    font-weight: 700;
    color: #3182f6;
    margin-bottom: 48px;
  }

  .footer-links {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 60px;
    margin-bottom: 60px;

    .footer-column {
      h4 {
        font-size: 18px;
        font-weight: 700;
        margin-bottom: 20px;
        color: #191f28;
      }

      a {
        display: block;
        text-decoration: none;
        color: #6b7684;
        font-size: 15px;
        margin-bottom: 12px;
        transition: color 0.2s;

        &:hover {
          color: #3182f6;
        }
      }
    }
  }

  .footer-bottom {
    padding-top: 40px;
    border-top: 1px solid #e5e8eb;
    text-align: center;
    color: #8b95a1;
    font-size: 14px;
  }
}

@media (max-width: 768px) {
  .footer {
    padding: 60px 20px 20px;

    .footer-links {
      grid-template-columns: 1fr;
      gap: 30px;
    }
  }
}
</style>
