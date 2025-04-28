<template>
    <div v-if="error">
        <p>Error: {{ error }}</p>
    </div>
    <div v-else-if="book">
        <div class="grid grid-cols-12 gap-10 mt-20">
            <div class="col-start-2">
                <NuxtLink to="/books"><svg xmlns="http://www.w3.org/2000/svg" width="37px" height="37px"
                        viewBox="0 0 24 24"><!-- Icon from Myna UI Icons by Praveen Juge - https://github.com/praveenjuge/mynaui-icons/blob/main/LICENSE -->
                        <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                            stroke-width="1.5" d="M19.5 12h-15m0 0l5.625-6M4.5 12l5.625 6"></path>
                    </svg></NuxtLink>
            </div>
            <div class="col-start-3 col-span-3 max-w-full">
                <NuxtImg :src="book.images" alt="Book Image" class="" />
            </div>
            <div class="col-start-3 col-span-3 space-y-4 overflow-y-auto max-h-[500px]">
                <img class="h-auto max-w-full" src="/images/vb2.jpg" alt="">
                <img class="h-auto max-w-full" src="/images/vb2achter.jpg" alt="">
                <!-- Add more images or content if needed -->
            </div>
            <div class=" col-start-7 col-span-4">
                <div class=" ">
                    <div class="text-3xl font-semibold">{{ book.title }}</div>
                    <div class="text-3xl font-semibold italic mt-3" v-if="book.field_author_creator">{{
                        book.field_author_creator }}
                    </div>
                </div>

                <div class="">
                    <div class="">
                        <div v-if="book.field_description" class="flex justify-between mt-4">
                            <div class="font-[rajdhani]"> description</div>
                            <div class="italic"> {{ book.field_description }}</div>
                        </div>
                        <div v-if="book.field_abstract" class="flex justify-between">
                            <div class="font-[rajdhani]"> abstract</div>
                            <div class="italic"> {{ book.field_abstract }}</div>
                        </div>
                        <div v-if="book.field_permalink">
                            <NuxtLink to={{book.field_permalink.value}} target="_blank">
                                <div class="buttonBack font-bold">
                                    Click here for more data on this publication and availability on Limo
                                </div>
                            </NuxtLink>
                        </div>
                        <button class="bg-black text-white font-[rajdhani] mt-4 p-1 text-l"> Available</button>
                    </div>


                    <div class="">
                        <hr>
                        <div v-if="book.field_author_creator" class="flex justify-between">
                            <div class="font-[rajdhani]"> author</div>
                            <div class="italic"> {{ book.field_author_creator }}</div>
                        </div>
                        <div v-if="book.field_collaborator" class="flex justify-between">
                            <div class="font-[rajdhani]"> collaborators</div>
                            <div class="italic"> {{ book.field_collaborator }}</div>
                        </div>
                        <div v-if="book.field_editor" class="flex justify-between">
                            <div class="font-[rajdhani]"> editor</div>
                            <div class="italic"> {{ book.field_editor }}</div>
                        </div>
                        <div v-if="book.field_date_of_publication" class="flex justify-between">
                            <div class="font-[rajdhani]"> date of publication</div>
                            <div class="italic"> {{ book.field_date_of_publication }}</div>
                        </div>
                        <div v-if="book.field_language" class="flex justify-between">
                            <div class="font-[rajdhani]"> language of publication</div>
                            <div class="italic"> {{ book.field_language }}</div>
                        </div>
                        <div v-if="book.field_number_of_pages" class="flex justify-between">
                            <div class="font-[rajdhani]"> number of pages</div>
                            <div class="italic"> {{ book.field_number_of_pages }}</div>
                        </div>

                        <hr>
                        <div v-if="book.field_other_titles" class="flex justify-between">
                            <div class="font-[rajdhani]"> other title</div>
                            <div class="italic"> {{ book.field_other_titles }}</div>
                        </div>
                        <div v-if="book.field_extent_of_the_edition" class="flex justify-between">
                            <div class="font-[rajdhani]"> exyend of the edition</div>
                            <div class="italic"> {{ book.field_language }}</div>
                        </div>
                        <div v-if="book.field_isbn" class="flex justify-between">
                            <div class="font-[rajdhani]"> ISBN</div>
                            <div class="italic"> {{ book.field_isbn }}</div>
                        </div>
                        <div v-if="book.field_genre_form" class="flex justify-between">
                            <div class="font-[rajdhani]"> genre</div>
                            <div class="italic" v-html="book.field_genre_form"> </div>
                        </div>
                        <div v-if="book.field_event" class="flex justify-between">
                            <div class="font-[rajdhani]"> event</div>
                            <div class="italic" v-html="book.field_event"></div>
                        </div>
                        <div v-if="book.field_source" class="flex justify-between">
                            <div class="font-[rajdhani]"> source</div>
                            <div class="italic" v-html="book.field_source"> </div>
                        </div>
                        <div v-if="book.field_subjects" class="flex ">
                            <div class="font-[rajdhani]"> subjects</div>
                            <div class="italic justify-end" v-html="book.field_subjects"> </div>
                        </div>
                        <div class="flex justify-between">
                            <div class="font-[rajdhani]"> id number</div>
                            <div class="italic"> {{ book.field_isbn }}</div>
                        </div>


                    </div>
                </div>
            </div>
            <!-- end Flexboxes -->
            <div class="">
                <favorites />
            </div>
        </div>

    </div>
    <div v-else>
        <p>Loading...</p>
    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import { useRoute } from 'vue-router';

const route = useRoute();
const book = ref(null);
const error = ref(null);

onMounted(async () => {
    const bookId = parseInt(route.params.id);

    try {
        const response = await fetch('/data/books.json');
        if (!response.ok) {
            throw new Error('Failed to fetch books data');
        }
        const data = await response.json();
        let found = false;
        for (let b of data) {
            // console.log(b.id)
            // console.log(bookId)
            if (b.id == bookId) {
                book.value = b;
                found = true;
                break;
            }
        }
        if (!found) {
            error.value = `Book with ID ${bookId} not found.`;
        }
    } catch (err) {
        error.value = `Error fetching data: ${err.message}`;
        console.error('Error fetching data:', err);
    }
});
</script>

<style>
.buttonBack {
    border: 1px solid #ccc;
    border-radius: .2em;
    margin-top: 1em;
    padding: .75em;
    width: max-content;
    max-width: 40vw;
}
</style>