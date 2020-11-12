<template>
  <div class="layout">
    <header class="header">
      <g-image src="~/layouts/assets/logo.svg" />

      <nav>
        <ul>
          <li>work</li>
          <li>art</li>
          <li>about</li>
          <li>contact</li>
        </ul>
      </nav>
    </header>
    <slot />
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style lang="scss">
nav ul {
  display: flex;
}
</style>
