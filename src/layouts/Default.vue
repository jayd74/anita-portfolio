<template>
  <div class="layout">
    <header class="header">
      <div class="navbar wrapper">
        <div class="logo">
          <g-image src="~/layouts/assets/logo.svg" />
          <span>Anita Ngo</span>
        </div>
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
    <footer>
      <div class="wrapper">
        <h2>LET’S CONNECT</h2>
        <div class="red-line"></div>

        <p>
          Hey! I’m currently seeking full-time opportunities. Feel free to get
          in touch.
        </p>

        <div class="social-icons">
          <a href="mailto: anita@anitango.com"
            ><g-image src="~/layouts/assets/email.svg"
          /></a>
          <a href="https://www.linkedin.com/in/anitango"
            ><g-image src="~/layouts/assets/linkedin.svg" alt="mail icon"
          /></a>
          <a href="https://dribbble.com/anitango"
            ><g-image src="~/layouts/assets/dribbble.svg"
          /></a>
          <a href="https://www.instagram.com/uxanita/"
            ><g-image src="~/layouts/assets/instagram.svg"
          /></a>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss">
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

.navbar,
.logo {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo span {
  text-transform: uppercase;
  margin-left: 32px;
  font-size: 24px;
  line-height: 36px;
}

nav ul {
  display: flex;
  color: #292929;

  li {
    list-style: none;
    text-transform: uppercase;
    padding: 50px;
    cursor: pointer;
    border-bottom: 10px solid transparent;
    transition: 0.3s;

    &:hover {
      border-bottom: 10px solid #ad0000;
    }
  }
}

footer {
  background: white;
  padding: 40px 0;

  .red-line {
    height: 10px;
    width: 105px;
    background: #ad0000;
    margin: 24px 0 40px;
  }

  .social-icons {
    display: flex;
    justify-content: space-between;
    width: 250px;
    margin: 20px 0;
    opacity: 1;

    img:hover {
      transition: 0.3s;
      opacity: 0.5;
    }
  }
}
</style>
