<template>
  <div class="my-auto">
    <h1 class="text-h2">
      Richard
      <span class="text-primary">Steen</span>
    </h1>

    <h3 class="h3">
      <vue-typer
        :text="['Software Engineer']"
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
      Austin · Texas ·
      <a href="mailto:name@email.com">richardjsteen@gmail.com</a>
    </div>
    <p class="h4">Software Engineer, Mountain Biker, Day Tripper</p>
    <ul class="list-inline list-social-icons mb-0">
      <li class="list-inline-item">
        <a target="blank" href="https://www.linkedin.com/in/richard-steen">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-linkedin-in fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank" href="https://github.com/rjsteen">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-github-alt fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>
