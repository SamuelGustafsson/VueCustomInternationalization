<template>
  <div class="hello">
    <h2>{{localised("hello")}}</h2>
    <h2>{{localised("goodbye")}}</h2>
    <button @click="activeLocale='en'">English</button>
    <button @click="activeLocale='sv'">Svenska</button>
  </div>
</template>

<script>
export default {
  name: "CustomTranslationsHandler",
  data() {
    return {
      activeLocale: "en",
      messages: {
        en: {
          hello: "Hello",
          goodbye: "Goodbye"
        },
        sv: {
          hello: "Hej",
          goodbye: "Hejdå"
        }
      }
    };
  },
  methods: {
    localised(key) {
      return this.messages[this.activeLocale][key];
    }
  }
};
</script>

