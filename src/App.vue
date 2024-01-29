<template lang="pug">
#app
  section.sheet.padding-10mm
    Brand
    hr
    h1 Vue App template
    .head1 Vue Templates
    ul
      li Using pug
  section.sheet.padding-10mm
    p Some other stuff...

</template>

<script>
import Brand from "./components/Head";
export default {
  components: { Brand }
};
</script>

<style>
@page {
  size: A5;
}

.head1 {
  background-color: red;
  text-align: center;
}
</style>