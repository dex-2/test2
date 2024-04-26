# test2


```
<template>
  <div class="mb-4 navbar">
    <div class="d-flex justify-space-between align-center">
      <NavbarLogo />
      <NavbarMenu :menuItems="menuItems" :activeTag="$route.meta.navTag" />
      <v-spacer />
      <SearchBar
        v-if="!searchClosed"
        v-model="searchText"
        @blur="searchClosed = true"
      />
      <ProfileButton class="profile-btn" />
    </div>
  </div>
</template>

<script>
// ... existing script block
</script>

<style scoped>
.navbar {
  padding: 0 16px; /* Adjust padding as necessary for your design */
}

/* Aligning the profile button to the center */
.profile-btn {
  margin-left: auto; /* Pushes the button to the right */
  align-self: center; /* Vertically centers the button */
}

/* Navbar Menu */
.nav-menu {
  margin-bottom: 0; /* Reducing bottom margin for the nav items */
}

/* If there is a specific class or element for the nav items within NavbarMenu, you may need to adjust their padding directly */
.nav-item {
  padding-bottom: 0; /* Example: Reducing padding at the bottom of each nav item */
}
</style>



```
