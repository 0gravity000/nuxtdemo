<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
          <a class="navbar-brand" href="#">Nuxt.js Demo</a>
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarNav"
            aria-controls="navbarNav"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon" />
          </button>
          <div id="navbarNav" class="collapse navbar-collapse">
            <ul class="navbar-nav">
              <li class="nav-item active mr-2">
                <NuxtLink
                  to="/"
                >
                  Welcome
                </NuxtLink>
              </li>
              <li class="nav-item mr-2">
                <NuxtLink
                  to="/sample-index"
                >
                  Sample
                </NuxtLink>
              </li>
              <li class="nav-item mr-2">
                <NuxtLink
                  to="/advance-index"
                >
                  Advance
                </NuxtLink>
              </li>
              <li class="nav-item mr-2">
                <NuxtLink
                  to="/htmlcss-index"
                >
                  HTML/CSS
                </NuxtLink>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
  </div>
</template>

<style>
</style>
