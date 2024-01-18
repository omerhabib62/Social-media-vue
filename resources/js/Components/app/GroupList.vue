<script setup>
import GroupItem from "@/Components/app/GroupItem.vue";
import TextInput from '@/Components/TextInput.vue';

const searchKeyword = '';
defineProps({

});
</script>

<template>
    <div class="px-3">
        <h2 class="text-2xl font-bold px-3 mb-4">My Groups</h2>
        <TextInput :modal-value="searchKeyword" placeholder="Type to search"/>
        <div class="py-8">
            <div v-if="false" class="text-gray-400 flex text-center">
                You are not joined to any group
            </div>

            <div v-else>
                <GroupItem
                    image="https://picsum.photos/100"
                    title="Laravel Developers"
                    description="lorem ipsum dolor sit amet, consectetur adipisicing elit."
                    />
                <GroupItem
                    image="https://picsum.photos/100"
                    title="Laravel Developers"
                    description="lorem ipsum dolor sit amet, consectetur adipisicing elit."
                    />
            </div>
        </div>
    </div>
</template>
