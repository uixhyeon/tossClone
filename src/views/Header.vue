<script setup>
import { ref, onMounted } from "vue";

const isScrolled = ref(false);
const isMenuOpen = ref(false);

onMounted(() => {
  window.addEventListener("scroll", () => {
    isScrolled.value = window.scrollY > 50;
  });
});

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

const closeMenu = () => {
  isMenuOpen.value = false;
};
</script>

<template>
  <header class="header" :class="{ scrolled: isScrolled }">
    <div class="header-container">
      <div class="logo">toss</div>
      <nav class="nav">
        <a href="#home">홈</a>
        <a href="#transfer">송금</a>
        <a href="#loan">대출</a>
        <a href="#credit">신용</a>
        <a href="#investment">투자</a>
        <a href="#payment">결제</a>
      </nav>
      <button class="hamburger" :class="{ active: isMenuOpen }" @click="toggleMenu">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </div>
    <nav class="mobile-nav" :class="{ open: isMenuOpen }">
      <a href="#home" @click="closeMenu">홈</a>
      <a href="#transfer" @click="closeMenu">송금</a>
      <a href="#loan" @click="closeMenu">대출</a>
      <a href="#credit" @click="closeMenu">신용</a>
      <a href="#investment" @click="closeMenu">투자</a>
      <a href="#payment" @click="closeMenu">결제</a>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  background: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid transparent;
  transition: all 0.3s;

  &.scrolled {
    background: rgba(255, 255, 255, 0.95);
    border-bottom-color: rgba(0, 0, 0, 0.1);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
  }

  .header-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    font-size: 28px;
    font-weight: 700;
    color: #3182f6;
  }

  .nav {
    display: flex;
    gap: 40px;

    a {
      text-decoration: none;
      color: #4e5968;
      font-size: 16px;
      font-weight: 500;
      transition: color 0.2s;

      &:hover {
        color: #3182f6;
      }
    }
  }

  .hamburger {
    display: none;
    flex-direction: column;
    background: none;
    border: none;
    cursor: pointer;
    padding: 0;
    gap: 6px;

    span {
      width: 25px;
      height: 3px;
      background-color: #191f28;
      border-radius: 2px;
      transition: all 0.3s;
      display: block;
    }

    &.active {
      span:nth-child(1) {
        transform: rotate(45deg) translate(10px, 10px);
      }

      span:nth-child(2) {
        opacity: 0;
      }

      span:nth-child(3) {
        transform: rotate(-45deg) translate(7px, -7px);
      }
    }
  }
}

.mobile-nav {
  display: none;
  position: fixed;
  top: 70px;
  left: 0;
  right: 0;
  background: rgba(255, 255, 255, 0.98);
  backdrop-filter: blur(10px);
  flex-direction: column;
  padding: 20px 40px;
  gap: 16px;
  z-index: 99;
  animation: slideDown 0.3s ease-out;

  a {
    text-decoration: none;
    color: #4e5968;
    font-size: 16px;
    font-weight: 500;
    padding: 12px 0;
    border-bottom: 1px solid #e5e8eb;
    transition: color 0.2s;

    &:last-child {
      border-bottom: none;
    }

    &:hover {
      color: #3182f6;
    }
  }

  &.open {
    display: flex;
  }
}

@keyframes slideDown {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 768px) {
  .header {
    .nav {
      display: none;
    }

    .hamburger {
      display: flex;
    }
  }

  .mobile-nav {
    top: 70px;
  }
}
</style>
