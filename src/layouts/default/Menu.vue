<template>

        <v-navigation-drawer
          expand-on-hover
          rail 
          permanent theme="dark"
        >
          <v-list>
            <v-list-item
              prepend-avatar="https://scontent.ftij2-1.fna.fbcdn.net/v/t39.30808-6/321306344_916095149757471_4948484563748121150_n.jpg?stp=cp6_dst-jpg&_nc_cat=101&ccb=1-7&_nc_sid=0debeb&_nc_ohc=5nUe9S0-VZ8AX-_h-F5&_nc_oc=AQk4tr39049Fxxnx2_LnmkIkhyYsSeQBCYg8I6fqc4Xaa_LRr1FSFIVQR46rGM2G4N8&_nc_ht=scontent.ftij2-1.fna&oh=00_AfAL1aM21X-ILsfbSD-JwDvz2frtMyEmp9w4QRykwuUaRg&oe=646C43D"
              title="Selene Muñoz"
              subtitle="compu@gmailcom"
            ></v-list-item>
          </v-list>
  
          <v-divider></v-divider>
  
          <v-list density="compact" nav>
            <v-list-item prepend-icon="mdi-home" title="Home" value="home" to="/"></v-list-item>
            <v-list-item prepend-icon="mdi-table" title="Table" value="table" to="/table"></v-list-item>
          </v-list>
        </v-navigation-drawer>
 
  </template>
  
  
