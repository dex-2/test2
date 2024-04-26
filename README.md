# test2


```

<template>
  <v-app-bar app dense class="navbar">
    <!-- Navbar content -->
    <v-toolbar-title class="d-flex align-center justify-start">
      <NavbarLogo />
      <NavbarMenu :menuItems="menuItems" :activeTag="$route.meta.navTag" />
    </v-toolbar-title>

    <v-spacer></v-spacer>

    <SearchBar
      v-if="!searchClosed"
      v-model="searchText"
      @blur="searchClosed = true"
      class="search-bar"
    />

    <ProfileButton class="profile-button" />

  </v-app-bar>
</template>

<script>
// ... Your existing script block
</script>

<style scoped>
.navbar {
  height: auto; /* Set the height to auto to adjust based on content */
}

/* Adjust the styles for your search bar and profile button as necessary */
.search-bar {
  /* Styles for search bar */
}

.profile-button {
  margin: auto 0; /* Vertically centers the profile button */
}

/* Update the NavbarMenu component if needed to adjust padding or margin */
.navbar-menu {
  margin-bottom: 0; /* Reduce bottom margin */
  /* Additional styling to bring the items closer to the bottom */
}

/* Additional global styles or modifications */
</style>


```
