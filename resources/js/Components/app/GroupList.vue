<script setup>
    import GroupItem from "@/Components/app/GroupItem.vue";
    import TextInput from '@/Components/TextInput.vue';
    import {ref} from   "vue";

    const searchKeyword = ref('');

    defineProps({

    });
    import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'
</script>

<template>
    <div class="px-3 bg-white rounded border py-3 lg:h-full overflow-hidden lg:flex lg:flex-col">
        <div class="block lg:hidden overflow-hidden flex flex-col h-full">
            <Disclosure v-slot="{ open }">            
                <DisclosureButton class="text-left">
                    <h2 class="text-xl font-bold mb-3">My Groups</h2>
                </DisclosureButton>
                <DisclosurePanel>
                    <TextInput :modal-value="searchKeyword" placeholder="Search" class="w-full"/>
                    <div class="mt-3 flex-1 overflow-auto">
                        <div v-if="false" class="text-gray-400 text-center p-3">
                            You are not joined to any group
                        </div>

                        <div v-else >
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
                </DisclosurePanel>            
            </Disclosure>
        </div>
        <div class="hidden lg:block overflow-hidden flex flex-col lg:h-full">
            <h2 class="text-xl font-bold mb-3">My Groups</h2>
            <TextInput :modal-value="searchKeyword" placeholder="Search" class="w-full"/>
            <div class="mt-3 flex-1 overflow-auto">
                <div v-if="false" class="text-gray-400 text-center p-3">
                    You are not joined to any group
                </div>

                <div v-else >
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
    </div>
</template>
