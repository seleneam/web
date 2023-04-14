<template>

        <v-navigation-drawer
          expand-on-hover
          rail 
          permanent theme="dark"
        >
          <v-list>
            <v-list-item
              prepend-avatar="https://scontent-sjc3-1.xx.fbcdn.net/v/t39.30808-6/275220313_4815796805204099_4477426810893078729_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=9-W-dkxnxIMAX-v0ncP&_nc_ht=scontent-sjc3-1.xx&oh=00_AfCdJZQwRy2Op6ug4GBflBRkf9ZDUVHZ0gZyScwhnnZRVQ&oe=64187CB1"
              title="Selene Muñoz"
              subtitle="@gmailcom"
            ></v-list-item>
          </v-list>
  
          <v-divider></v-divider>
  
          <v-list density="compact" nav>
            <v-list-item prepend-icon="mdi-home" title="Home" value="home" to="/"></v-list-item>
            <v-list-item prepend-icon="mdi-table" title="Table" value="table" to="/table"></v-list-item>
          </v-list>
        </v-navigation-drawer>
 
  </template>
  
  
