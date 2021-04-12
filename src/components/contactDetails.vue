<template>
  <div class="contactDetails__container">
    <h2>Looking to contact someone quickly? Look below!</h2>
    <div class="contacts__container">
      <div
        v-for="contact in contacts"
        :key="contact.name"
        class="contact__container"
      >
        <h3>{{ contact.name }}</h3>
        <div>{{ contact.person }}</div>
        <div>{{ contact.phone }}</div>
        <div>{{ contact.email }}</div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "contactDetails",
  data() {
    return {
      contacts: [
        {
          name: "Parts Dept",
          person: "Ryan Goodhue",
          phone: "920-927-3854",
          email: "",
        },
        {
          name: "Shop Dept",
          person: "Neel Huffman",
          phone: "920-927-3851",
          email: "",
        },
        {
          name: "Road Dept",
          person: "Zoom Neuamn",
          phone: "920-927-3851",
          email: "",
        },
      ],
    };
  },
};
</script>

<style scoped>
h2 {
  color: rgb(211, 211, 211);
  padding: 8px;
  margin-left: 4em;
  margin-right: 4em;
  border-bottom: 1px solid rgb(211, 211, 211);
}
.contactDetails__container {
  background: #9d1d21;
  text-align: center;
}
.contacts__container {
  display: flex;
  padding: 18px 0;
}
.contact__container {
  color: #1c1a1a;
  width: 33.33%;
  text-align: center;
}
</style>