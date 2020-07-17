<template>
  <div class="content-wrapper bg-background-primary font-sans text-copy-primary leading-normal flex flex-col min-h-screen" :class="theme">
    <header class="sticky top-0 z-10 w-full border-t-14 border-black">

    </header>

    <div class="flex-grow">
      <slot/>



    </div>
    <footer class="bg-black text-white">
      <div class="container mx-auto flex flex-col lg:flex-row items-center justify-between py-8">
        <div class="mb-8 lg:mb-0">
          <div>Copyright © {{ new Date().getFullYear() }} Oui Très Jolie. All rights reserved.     
</div>
         </div>
         </div>
    </footer>
    </div>

    </template>

    <static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>

</script>

<style src="../css/main.css" />