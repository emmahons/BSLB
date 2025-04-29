<template>
  <div class="grid grid-cols-12 gap-10 mt-20">
    <div class="col-start-2 col-span-10">
      <h1 class="title"> Peeters collection</h1>
    </div>
  </div>
  <div class="grid grid-cols-12 gap-10">
    <ul
      class=" grid col-start-3 col-span-11 lg:grid-cols-4 sm:grid-cols-2 gap-x-10 gap-y-4  auto-rows-min overflow-hidden ">
      <li v-for="book in books" :key="book.id" class="">
        <div class="text-xl font-bold col-span-2 ">
          <RouterLink :to="`/books/${book.id}`">
            <NuxtImg :src="book.image" alt="Book Image" class="col-span-2" />
          </RouterLink>
        </div>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
const books = ref([]);
onMounted(async () => {
  try {
    const response = await fetch('/data/books.json');
    const data = await response.json();
    books.value = data.map(book => ({
      id: book.id,
      title: book.title,
      image: book.image
    }));
  } catch (error) {
    console.error('Error fetching data:', error);
  }
});
</script>
