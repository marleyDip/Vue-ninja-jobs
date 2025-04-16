<template>
  <div class="home">
    <h1>Vue Router</h1>
    <ul>
      <li>
        Routing in Vue is used to navigate the Vue application, and it happens
        on the client side (in the browser) without full page reload, which
        results in a faster user experience. Routing is a way to navigate,
        similar to how we have used dynamic components earlier. With routing we
        can use the URL address to direct someone to a specific place in our Vue
        application.
      </li>
      <li>
        Vue Router is the official router for Vue.js. It enables navigation
        between different components in a Vue application, allowing for a
        single-page application (SPA) experience.
      </li>
      <li>
        Vue Router allows you to define routes in your application, which map
        URLs to components. This means that when a user navigates to a specific
        URL, the corresponding component is rendered without the need for a full
        page reload.
      </li>
    </ul>
    <h5 style="text-align: justify; justify-content: center">
      Router link is used to navigate between different components in a Vue
      application. It is a built-in component provided by Vue Router that allows
      you to create links to different routes in your application. The
      router-link component is similar to the HTML anchor tag (a), but it
      provides additional functionality specific to Vue Router. When a user
      clicks on a router-link, Vue Router intercepts the click event and updates
      the URL in the browser's address bar without reloading the page. This
      allows for a smoother user experience, as the application can update the
      displayed component without the need for a full page refresh. The
      router-link component can be used to navigate to different routes in your
      application, and it can also accept parameters to pass data to the
    </h5>
    <!-- <p>
      <router-link to="/about">Go to Jobs</router-link>
    </p> -->
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "HomeView",
  components: {},
};
</script>

<style scoped>
li {
  margin: 10px;
  padding: 10px;
  border: 1px solid #6ed711;
  border-radius: 5px;
  background-color: #f9f9f9;
  list-style-type: lower-greek;
  font-size: 16px;
  line-height: 1.5;
  color: #333;
  transition: background-color 0.3s ease;
  cursor: pointer;
}
</style>
