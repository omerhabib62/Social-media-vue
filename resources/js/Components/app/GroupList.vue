<script setup>
    import GroupItem from "@/Components/app/GroupItem.vue";
    import TextInput from '@/Components/TextInput.vue';
    import {ref} from   "vue";

    const searchKeyword = ref('');

    defineProps({

    });
</script>

<template>
    <div class="px-3">
        <h2 class="text-2xl font-bold mb-3">My Groups</h2>
        <TextInput :modal-value="searchKeyword" placeholder="Search"/>
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
