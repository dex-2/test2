# test2


```
<template>
  <div class="navbar-container">
    <div class="navbar-content">
      <div class="navbar-column logo-column">
        <NavbarLogo />
      </div>
      <div class="navbar-column nav-items-column">
        <NavbarMenu :menuItems="menuItems" :activeTag="$route.meta.navTag" />
      </div>
      <div class="navbar-column profile-button-column">
        <ProfileButton />
      </div>
    </div>
  </div>
</template>

<script>
// ... existing script content
</script>

<style scoped>
.navbar-container {
  display: flex;
  align-items: center; /* This centers the navbar content vertically */
  justify-content: space-between; /* This spreads out the logo, nav items, and profile button */
}

.navbar-content {
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.navbar-column {
  display: flex;
  align-items: flex-end; /* Aligns items to the bottom */
}

.logo-column {
  /* Logo column styles */
}

.nav-items-column {
  flex-grow: 1; /* Allows this column to take up the available space */
  /* Additional styles to position the nav items */
}

.profile-button-column {
  display: flex;
  align-items: center; /* This will vertically center the profile button */
  justify-content: flex-end; /* Aligns the profile button to the right */
}

/* You might need to add additional styles or adjust the existing ones based on your design */
</style>

```
