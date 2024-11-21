<template>
  <section>
    <profile />
    <menumobile />
    <div class="main-content max-width-1160px mx-auto">
      <menudesktop />
      <Nuxt />
    </div>
  </section>
</template>

<style>
.main-content {
  display: flex;
  flex: 1;
}

menudesktop {
  flex-shrink: 0;
  width: 200px;
  background-color: #f4f4f4;
}

Nuxt {
  flex-grow: 1;
}
</style>
