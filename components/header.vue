<template>
  <v-layout>
    <v-navigation-drawer app expand-on-hover rail clipped>
      <v-list>
        <v-list-item
            prepend-avatar="../public/profile_picture.jpg"
            subtitle="PARPAILLON Olivier"
            title="A propos de moi"
        ></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-folder" title="Mes formations" value="myfiles"></v-list-item>
        <v-list-item prepend-icon="mdi-account-multiple" title="Mon expériences" value="shared"></v-list-item>
        <v-list-item prepend-icon="mdi-star" title="Mes compétences" value="starred"></v-list-item>
      </v-list>
    </v-navigation-drawer>
  </v-layout>
</template>
