<template>
  <div>
    <button type="submit" @click.prevent="deleteMessage">X</button>
  </div>
</template>


<script>
import axios from "axios";

export default {
  name: "deleteMessage",
  props: {
    id: Number,
  },
  data() {
    return {
      token: "",
    };
  },
  methods: {
    deleteMessage() {
      let token = localStorage.getItem("token");
      axios
        .delete("http://localhost:3000/api/messages/" + this.id, {
          headers: { Authorization: "Bearer " + token },
        })
        .then(() => {
          alert("Votre message a bien été supprimé !");
          document.location.reload();
        })
        .catch((error) => {
          console.log({ error });
        });
    },
  },
};
</script>

<style scoped>
button {
  background-color: red;
  color: white;
}
</style>