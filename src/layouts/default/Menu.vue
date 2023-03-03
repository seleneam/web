<template>

        <v-navigation-drawer
          expand-on-hover
          rail 
          permanent theme="dark"
        >
          <v-list>
            <v-list-item
              prepend-avatar="https://scontent-sjc3-1.xx.fbcdn.net/v/t39.30808-6/323578176_1179565286019710_119805909729287364_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=8zoZxmYBvqoAX8TkgZT&tn=WID98KtWEApSNEA4&_nc_ht=scontent-sjc3-1.xx&oh=00_AfBxqepKitHHCbpSoOwpT5eInLj1615_wg-CpCckY4mw8w&oe=63FC32A2"
              title="Selene Muñoz"
              subtitle="selene_directioner@gmailcom"
            ></v-list-item>
          </v-list>
  
          <v-divider></v-divider>
  
          <v-list density="compact" nav>
            <v-list-item prepend-icon="mdi-home" title="Home" value="home" to="/"></v-list-item>
            <v-list-item prepend-icon="mdi-table" title="Table" value="table" to="/table"></v-list-item>
          </v-list>
        </v-navigation-drawer>
 
  </template>
  
  
