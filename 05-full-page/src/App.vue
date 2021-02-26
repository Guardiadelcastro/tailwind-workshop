<template>
  <Header />
  <main class="px-4 py-10 sm:px-10 lg:max-w-5xl lg:mx-auto">
    <div
      class="flex justify-between items-center border-b-2 border-emerald-500 pb-3 border-dashed"
    >
      <h1 class="text-3xl font-semibold text-emerald-500">Inbox</h1>
      <OutlineButton>New Email</OutlineButton>
    </div>
    <div>
      <ul class="py-4">
        <template v-for="email in emails" :key="email.id">
          <EmailItem :email="email" />
        </template>
      </ul>
    </div>
  </main>
  <Footer />
</template>

<script setup>
import { ref } from "vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
import OutlineButton from "./components/OutlineButton.vue";
import EmailItem from "./components/EmailItem.vue";

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
const emails = ref([
  {
    id: "bd88189f-d479-4c8d-a850-0051cd92a41e",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Angelina",
    subject: "Steel mission-critical Hat",
    date: "Thu Feb 25 2021 19:08:49 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "e2425ea0-e438-444f-89f5-91bc72b4fecf",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Yasmine",
    subject: "optimizing",
    date: "Fri Feb 26 2021 02:32:02 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "df06fd09-71cb-4d0b-9c01-362d7efd6729",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Dorian",
    subject: "blue Sleek Designer",
    date: "Thu Feb 25 2021 22:08:13 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "35721718-8dd0-459e-8fd5-0537732358d7",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Darius",
    subject: "application invoice Agent",
    date: "Fri Feb 26 2021 03:26:26 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "deda594e-bd5b-4bef-8a9b-d036594d6829",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Mose",
    subject: "Manager compress",
    date: "Thu Feb 25 2021 19:37:40 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "9a94c45e-2da2-4f5a-b170-41746ed03107",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Mack",
    subject: "El Keyboard",
    date: "Thu Feb 25 2021 08:37:29 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "f941589d-cf40-4b94-b514-ca90e4debe5d",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Antonetta",
    subject: "bandwidth-monitored pixel holistic",
    date: "Thu Feb 25 2021 23:57:40 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "d6de0430-e7f1-43c8-8830-641c4bb5baa1",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Reginald",
    subject: "index",
    date: "Thu Feb 25 2021 09:06:17 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "aff10c0c-e8e8-43e2-b67f-c4b8573b0ef4",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Freddie",
    subject: "firewall Camp",
    date: "Thu Feb 25 2021 16:51:55 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "42183fa3-da32-4f60-a766-8b4fefb23a7b",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Keith",
    subject: "cross-platform Cotton",
    date: "Fri Feb 26 2021 04:54:02 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "31e23504-96c2-408c-93b8-07a6a09b7944",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Jana",
    subject: "Singapore Metal",
    date: "Thu Feb 25 2021 17:20:33 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
  {
    id: "e10313b1-8b55-44eb-9528-e97fcddca464",
    img: "https://randomuser.me/api/portraits/men/35.jpg",
    name: "Kameron",
    subject: "Brand ability",
    date: "Thu Feb 25 2021 22:24:34 GMT+0000 (Western European Standard Time)",
    tag: "Priority",
  },
]);
</script>

<style lang="postcss">
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>
