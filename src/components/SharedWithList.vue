<template>
    <ul class="list-group rounded-0 list-group-horizontal justify-content-center pb-2">
      <li v-for="(avatar, index) in avatars" :key="index" class="list-group-item border-0 d-flex align-items-center p-0">
        <img :src="avatar.src" :alt="avatar.alt" class="rounded-circle me-n2" width="45" />
      </li>
    </ul>
  </template>
  
  <script>
  export default {
    data() {
      return {
        avatars: [
          {
            src: "https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-8.webp",
            alt: "Avatar 1",
          },
          {
            src: "https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-3.webp",
            alt: "Avatar 2",
          },
          {
            src: "https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-5.webp",
            alt: "Avatar 3",
          },
          {
            src: "https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-6.webp",
            alt: "Avatar 4",
          },
        ],
      };
    },
  };
  </script>
  