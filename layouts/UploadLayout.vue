<template>
  <div
    class="bg-[#F8F8F8] h-[100vh]"  
  >
  <TopNav />
    <div>
      <SideNavMain />
    </div>
    <slot />
  </div>
</template>

<script setup>
const route = useRoute()
</script>
