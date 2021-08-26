<template>
  <div class="contaainer mt-5">
    <div class="home">
      <trainer-card />
      <img alt="Vue logo" src="../assets/logo.png" />
      <generations-list />
      <HFooter />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import GenerationsList from "@/components/GenerationsList.vue";
import TrainerCard from "@/components/TrainerCard.vue";
import HFooter from "vue-hacktiv8-footer";

export default {
  name: "Home",
  components: {
    GenerationsList,
    TrainerCard,
    HFooter
  },
};
</script>
