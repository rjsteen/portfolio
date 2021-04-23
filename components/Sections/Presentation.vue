<template>
  <div class="my-auto">
    <h1 class="text-h3">
      Richard
      <span class="text-primary">Steen</span>
    </h1>

    <h3 class="text-h6">
      <vue-typer
        :text="['Software Engineer', 'Mountain Biker', 'Day Tripper']"
        :repeat="Infinity"
        :shuffle="true"
        initial-action="typing"
        :pre-type-delay="100"
        :type-delay="82"
        :pre-erase-delay="2000"
        :erase-delay="30"
        erase-style="backspace"
        :erase-on-complete="false"
        caret-animation="blink"
      ></vue-typer>
    </h3>

    <div class="subheading mb-5">
      Austin, TX ·
      <a href="mailto:name@email.com">richardjsteen@gmail.com</a>
    </div>
    <p>Love to learn, explore, and try new things</p>
    <ul class="list-inline list-social-icons">
      <!-- <li class="list-inline-item">
        <a href="#">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-facebook-f fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li> -->

      <li class="list-inline-item">
        <a target="blank">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-linkedin-in fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-github-alt fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
    </ul>
    <v-divider></v-divider> <br /><br />
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>
