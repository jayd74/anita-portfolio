<template>
  <div class="layout">
    <header class="header">
      <div class="navbar wrapper">
        <g-image src="~/layouts/assets/logo.svg" />

        <nav>
          <ul>
            <li>work</li>
            <li>art</li>
            <li>about</li>
            <li>contact</li>
          </ul>
        </nav>
      </div>
    </header>
    <slot />
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@400;700;900&display=swap");

html {
  font-family: "Nunito", sans-serif;
}

.wrapper {
  margin: 0 auto;
  max-width: 375px;
  width: 100%;

  @media screen and (min-width: 1024px) {
    max-width: 960px;
  }

  @media screen and (min-width: 1440px) {
    max-width: 1024px;
  }
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #fafafa;
  width: 100%;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

.navbar {
  display: flex;
  justify-content: space-between;
}

nav ul {
  display: flex;

  li {
    list-style: none;
    text-transform: uppercase;
    padding: 50px;
    cursor: pointer;
    border-bottom: 10px solid transparent;

    &:hover {
      border-bottom: 10px solid #ad0000;
    }
  }
}
</style>
