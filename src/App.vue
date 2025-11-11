<script setup>
import Header from "./views/Header.vue";
import HeroSection from "./views/HeroSection.vue";
import HomeSection from "./views/HomeSection.vue";
import TransferSection from "./views/TransferSection.vue";
import LoanSection from "./views/LoanSection.vue";
import CreditSection from "./views/CreditSection.vue";
import InvestmentSection from "./views/InvestmentSection.vue";
import ConvenienceSection from "./views/ConvenienceSection.vue";
import PaymentSection from "./views/PaymentSection.vue";
import BusinessSection from "./views/BusinessSection.vue";
import Footer from "./views/Footer.vue";
</script>

<template>
  <div class="app">
    <Header />
    <HeroSection />
    <HomeSection />
    <TransferSection />
    <LoanSection />
    <CreditSection />
    <InvestmentSection />
    <ConvenienceSection />
    <PaymentSection />
    <BusinessSection />
    <Footer />
  </div>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans KR",
    sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #191f28;
  background: #fff;
}

.app {
  width: 100%;
  overflow-x: hidden;
}
</style>
