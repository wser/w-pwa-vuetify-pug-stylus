<template lang="pug">
v-card(color='grey lighten-4' flat height='200px')
  v-toolbar(color='grey darken-1' dark)
    v-toolbar-side-icon
    v-menu(:nudge-width='100')
      template(v-slot:activator='{ on }')
        v-toolbar-title(v-on='on')
          span All
          v-icon(dark) arrow_drop_down
      v-list
        v-list-tile(v-for='item in items' :key='item' @click)
          v-list-tile-title(v-text='item')
    v-spacer
    v-btn(icon to='/')
      v-icon search  
    v-btn(icon to='/about')
      v-icon favorite
    v-btn(icon)
      v-icon more_vert
</template>
