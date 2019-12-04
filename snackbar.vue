<template>
  <div class="snackbar">
      <v-navigation-drawer  expand-on-hover clipped permanent color="#0d98ba">
          <template v-slot:prepend >
              <v-list> 
                <v-list-item>
                  <v-list-item-avatar size="65" color="grey">
                    <v-img src=""></v-img>
                  </v-list-item-avatar>

                  <h1></h1>
                    
                </v-list-item>
              </v-list>
          </template>

          <v-divider></v-divider>

          <v-list nav>
            <v-list-item link to="/dashboard">
              <v-list-item-icon>
                  <v-icon color="white" size="60">mdi-home</v-icon>
              </v-list-item-icon>
              <v-list-item-title size="60" class="white--text">Dashboard</v-list-item-title>
            </v-list-item>
            <v-list-item link to="/profile">
              <v-list-item-icon>
                  <v-icon color="white" size="60">mdi-account-supervisor</v-icon>
              </v-list-item-icon>
              <v-list-item-title size="60" class="white--text">Account</v-list-item-title>
            </v-list-item>
            
            <v-list-item link to="/all-courses">
              <v-list-item-icon>
                  <v-icon color="white" size="60">mdi-library-books</v-icon>
              </v-list-item-icon>
              <v-list-item-title size="60" class="white--text">Courses</v-list-item-title>
            </v-list-item>
            <v-list-item link>
              <v-list-item-icon>
                  <v-icon color="white" size="60">mdi-tune</v-icon>
              </v-list-item-icon>
              <v-list-item-title class="white--text" size="60">Settings</v-list-item-title>
            </v-list-item>
            
            <v-list-item link class="help">
              <v-list-item-icon>
                  <v-icon color="white" size="60">mdi-help</v-icon>
              </v-list-item-icon>
              <v-list-item-title class="white--text">help</v-list-item-title>
            </v-list-item>
        </v-list>
      </v-navigation-drawer>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        drawer: true,
        mini: true
      }
    },
  }
</script>

<style scoped>

.snack {
  width: 300px !important;
  height: 100%;
}

.help {
  margin-top: 60% !important;
}

</style>