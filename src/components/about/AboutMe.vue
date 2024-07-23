<script>
export default {
  setup() {
    return {
      bios: [
        {
          id: 1,
          bio: "👋 Hi, I’m @Bwirabuciza29 👀 I’m interested in creating intuitive and visually appealing user interfaces, solving design challenges, and exploring new design trends. 🌱 I’m currently learning advanced animation techniques and mastering component-based architecture in Vue.js. 💞️ I’m looking to collaborate on projects that push the boundaries of UI/UX design, where I can contribute my expertise in Vue.js development. 📫 How to reach me: You can reach me via outlook at achilleblondy@outlook.fr or connect with me on LinkedIn https://www.linkedin.com/in/bwirabuciza-blondy-58b137245. 😄 Pronouns: He/Him ⚡ Fun fact: I'm an avid hiker and find inspiration for my designs in nature's patterns and colors.",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
    <!-- About profile image -->
    <div class="w-full sm:w-1/4 mb-7 sm:mb-0">
      <img src="@/assets/images/blondy.jpg" class="rounded-xl w-96" alt="" />
    </div>

    <!-- About details -->
    <div class="w-full sm:w-3/4 text-left">
      <p
        v-for="bio in bios"
        :key="bio.id"
        class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg text-justify"
      >
        {{ bio.bio }}
      </p>
    </div>
  </div>
</template>
