<script setup lang="ts">
import ChatBubble from './ChatBubble.vue';

</script>

<template>

    <div class="flex-1 overflow-y-auto p-4">
        <div class="flex flex-col space-y-2">
            <!-- Messages go here -->
            <ChatBubble :its-mine="true" :message="'Hola que tal?'" />
            <ChatBubble :its-mine="false" :message="'no'"
                image="https://yesno.wtf/assets/yes/5-64c2804cc48057b94fd0b3eaf323d92c.gif" />
        </div>
    </div>

</template>