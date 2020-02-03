<template>
  <div class="aligner">
    <div class="main">
      <div class="title">
        <h2> Hey! I'm Elly- </h2>
      </div>
      <div class="text-body">
        <p>I’m an aspiring artist/dev/designer/physics nerd in high school. I’ve interned at 12345,
          678, and a few other places- it’s not uncommon to see me rolling around!</p>
        <p>I am one of the cofounders of UXHouse (also lovingly known as Waffle House), a community
          where anybody interested in UX can collaborate, share, discuss, and contribute.</p>
      </div>

      <div class="footer-bottom">
        <small>psst, have you seen my design system?</small>
        <div class="push"></div>
        <div class="right">
          <Link />
          <Github />
          <Mail />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Link from '@/components/Link.vue';
import Github from '@/components/Github.vue';
import Mail from '@/components/Mail.vue';

export default {
  name: 'Main',
  components: {
    Link,
    Github,
    Mail,
  },
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .aligner {
    margin-top: 4vh;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    position: relative;
  }

  .main {
    display: flex;
    flex-direction: column;
    width: 80vw;
    height: 80vh;
    max-height: 80vh;
    background-color: #fff;
    padding: 1em;
  }

  .text-body {
    display: flex;
    flex-grow: 1;
  }

  .footer-bottom {
    margin-bottom: auto;
  }

  .push {
    margin-left: auto;
  }

</style>
