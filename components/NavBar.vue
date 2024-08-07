<template>
  <nav class="navbar">
    <div class="navbar-container">
      <nuxt-link to="/" class="navbar-logo">
        <img src="/assets/logo.png" alt="Logo" />
      </nuxt-link>

      <nuxt-link to="/" class="navbar-logo-text">
        <h1>LOGO</h1>
      </nuxt-link>
      <ul class="nav-menu">
        <li class="nav-item">
          <nuxt-link to="/" class="nav-links">
            <img src="/assets/search-normal.png" alt="Search" />
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/about" class="nav-links">
            <img src="/assets/heart.png" alt="Favorites" />
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/services" class="nav-links">
            <img src="/assets/profile.png" alt="Profile" />
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/contact" class="nav-links">
            <img src="/assets/shopping-bag.png" alt="Cart" />
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/contact" class="nav-links">
            <img src="/assets/Language.png" alt="Language" />
          </nuxt-link>
        </li>
      </ul>
    </div>

    <div class="navbar-container second-nav">
      <ul class="nav-menu-second">
        <li class="nav-item">
          <nuxt-link to="/" class="nav-links">Shop</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/about" class="nav-links">Skills</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/services" class="nav-links">Stories</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/contact" class="nav-links">About</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/contact" class="nav-links">Contact Us</nuxt-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-size: 1.2rem;
  width: 100%;
  padding: 0 20px;
}

.navbar-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  max-width: 1440px;
}

.second-nav {
  text-align: center;
  align-items: center;
  justify-content: center;
  border-bottom: 1px solid #ddd;
}

.navbar-logo {
  justify-self: start;
  margin-left: 20px;
  cursor: pointer;
  text-decoration: none;
  font-size: 1.5rem;
}

.navbar-logo-text {
  font-family: Inter;
  font-size: 36px;
  font-weight: 800;
  line-height: 43.57px;
  letter-spacing: 1px;
  text-align: left;
  text-decoration: none;
  color: #000000;
}

.nav-menu {
  display: flex;
  align-items: center;
  list-style: none;
  text-align: center;
}

.nav-menu-second {
  display: flex;
  align-items: center;
  list-style: none;
  width: 50%;
}

.nav-links {
  display: flex;
  align-items: center;
  text-decoration: none;
  padding: 0 1rem;
  height: 100%;
  cursor: pointer;
  color: #000000;
  font-family: 'Norm', sans-serif;
  font-size: 20px;
  font-weight: 700;
  line-height: 24px;
  letter-spacing: 1px;
  text-align: left;
}

.nav-links:hover {
  border-bottom: 2px solid #fff;
}

@media (max-width: 768px) {
  .navbar-container {
    flex-direction: column;
  }

  .nav-menu {
    display: none;
  }

  .navbar-logo-text {
    font-size: 28px;
  }
}

@media (max-width: 480px) {
  .navbar-logo img {
    width: 40px;
    height: 40px;
  }

  .navbar-logo-text {
    font-size: 24px;
  }

  .nav-links {
    font-size: 16px;
    padding: 0.5rem;
  }
}
</style>
