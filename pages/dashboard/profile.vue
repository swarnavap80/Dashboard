<template>
    <div class="flex flex-col items-center justify-center h-screen">
        <h1 class="text-3xl font-bold">Profile</h1>
        <account-information />

        <edit-account-modal v-if="modal && modal.type === 'edit-account'" />
    </div>
</template>

<script lang="ts" setup>
// Interface
interface Modal {
    type: string;
    data: string;
}

const modal = ref(null as Modal | null);
</script>