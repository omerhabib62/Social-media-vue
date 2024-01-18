<script setup>
import FollowingItem from "@/Components/app/FollowingItem.vue";
import TextInput from '@/Components/TextInput.vue';
import {ref} from   "vue";

const searchKeyword = ref('');
defineProps({

});
</script>

<template>
    <div class="px-3">
        <h2 class="text-2xl font-bold mb-3">My Friends</h2>
        <TextInput :modal-value="searchKeyword" placeholder="Search"/>
        <div class="py-8">
            <div v-if="false" class="text-gray-400 flex text-center">
                You don't have any friends yet.
            </div>

            <div v-else>
                <FollowingItem
                    image="https://picsum.photos/100"
                    title="John Doe"
                    />
                <FollowingItem
                    image="https://picsum.photos/100"
                    title="Denzel Washington"
                    />
            </div>
        </div>
    </div>
</template>
