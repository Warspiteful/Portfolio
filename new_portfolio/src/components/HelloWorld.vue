<template>
  <v-app>
    <v-app-bar color="primary" dark flex>
      <v-spacer></v-spacer>
      <v-toolbar-title><h1>Justin Almendral</h1></v-toolbar-title>
      <v-spacer></v-spacer>

      <v-row slot="extension" class="text-center">
        <v-col cols="4">

          <h3>Phone Number: 201-961-3196</h3>

        </v-col>
        <v-spacer></v-spacer>
        <v-col cols="4">

          <h3>Email: jalmendral24@gmail.com</h3>

        </v-col>
        <v-col cols="4">

          <h3>Availability: May 2022 - August 2022</h3>

        </v-col>

      </v-row>
    </v-app-bar>
    <v-container>

      <v-row class="text-left">
        <v-col cols="6">
          <v-img :src="require('../assets/logo.svg')" class="my-3" contain height="200" />

        </v-col>
        <v-col cols="4">
        <h1>I'm Justin Almendral</h1>
        <p>My name is Justin Almendral (they/them). I'm a third year Computer Engineering student at Northeastern University. I make games and websites, exploring new ideas.</p>
        <p>I'm currently the Social Chair of Northeastern's Game Development Club, organizing game jams and events for the Northeastern Game Development Community.</p>
        <p>I tend towards JRPGs, Card Games, and Visual Novels. My current favorite game is Library of Ruina.</p>

        </v-col>
                  </v-row>

 <v-row class="text-center">
    
        <v-col cols="12">
          <v-img :src="require('../assets/logo.svg')" class="my-3" contain height="200" />
        </v-col>

        <v-col class="mb-4">
          <h1 class="display-2 font-weight-bold mb-3">
            Welcome to Vuetify
          </h1>

          <p class="subheading font-weight-regular">
            For help and collaboration with other Vuetify developers,
            <br>please join our online
            <a href="https://community.vuetifyjs.com" target="_blank">Discord Community</a>
          </p>
        </v-col>

        <v-col class="mb-5" cols="12">
          <h2 class="headline font-weight-bold mb-3">
            What's next?
          </h2>

          <v-row justify="center">
            <a v-for="(next, i) in whatsNext" :key="i" :href="next.href" class="subheading mx-3" target="_blank">
              {{ next.text }}
            </a>
          </v-row>
        </v-col>

        <v-col class="mb-5" cols="12">
          <h2 class="headline font-weight-bold mb-3">
            Important Links
          </h2>

          <v-row justify="center">
            <a v-for="(link, i) in importantLinks" :key="i" :href="link.href" class="subheading mx-3" target="_blank">
              {{ link.text }}
            </a>
          </v-row>
        </v-col>

        <v-col class="mb-5" cols="12">
          <h2 class="headline font-weight-bold mb-3">
            Ecosystem
          </h2>

          <v-row justify="center">
            <a v-for="(eco, i) in ecosystem" :key="i" :href="eco.href" class="subheading mx-3" target="_blank">
              {{ eco.text }}
            </a>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
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
    whatsNext: [
      {
        text: 'Explore components',
        href: 'https://vuetifyjs.com/components/api-explorer',
      },
      {
        text: 'Select a layout',
        href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
      },
      {
        text: 'Frequently Asked Questions',
        href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
      },
    ],
  }),
}
</script>
