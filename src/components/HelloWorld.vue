<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/dog-headshot.jpg')"
          class="my-3"
          contain
          height="300"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          HI, It's Shiba here!
        </h1>
        <h2>
          There are all about my Travel and Wtire!
        </h2>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          My Social Media
        </h2>

        <v-row justify="center">
          <a
            v-for="(next, i) in socialMedia"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      socialMedia: [
        {
          text: 'Instagram',
          href: 'https://www.instagram.com/shenghung0514/',
        },
        {
          text: 'Youtube',
          href: 'https://www.youtube.com/channel/UCVFsHQFNWphAG2XCjqxEwNA/featured',
        },
        {
          text: 'Facebook',
          href: 'https://www.facebook.com/shenghung.tsai.1',
        },
      ],
    }),
  }
</script>
