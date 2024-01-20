<script setup>
import FollowingItem from "@/Components/app/FollowingItem.vue";
import TextInput from '@/Components/TextInput.vue';
import {ref} from   "vue";

const searchKeyword = ref('');
defineProps({

});
</script>

<template>
    <div class="px-3 bg-white rounded border py-3 h-[300px] lg:h-full overflow-hidden flex flex-col">
        <h2 class="text-xl font-bold mb-3">Following</h2>
        <TextInput :modal-value="searchKeyword" placeholder="Search" class="w-full"/>
        <div class="mt-3 flex-1 overflow-auto">
            <div v-if="false" class="text-gray-400 text-center p-3">
                You are not following yet.
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
                <FollowingItem
                    image="https://picsum.photos/100"
                    title="John Doe"
                    />
                <FollowingItem
                    image="https://picsum.photos/100"
                    title="Denzel Washington"
                    /> <FollowingItem
                    image="https://picsum.photos/100"
                    title="John Doe"
                    />
                <FollowingItem
                    image="https://picsum.photos/100"
                    title="Denzel Washington"
                    /> <FollowingItem
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
