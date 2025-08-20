<script setup lang="ts">
import ChatMessages from '@/components/chat/ChatMessages.vue';
import MessageBox from '@/components/chat/MessageBox.vue';
import type { ChatMessage } from '@/interfaces/chat-message.interface';
import { ref } from 'vue';

const messages = ref<ChatMessage[]>([
    {
        id: new Date().getTime(),
        message: 'Hola que tal?',
        itsMine: true,
    },
    {
        id: new Date().getTime(),
        message: 'Quieres ir por cafe?',
        itsMine: true,
    },
    {
        id: new Date().getTime() + 1,
        message: 'Bien, gracias y tu?',
        itsMine: false,
        image: 'https://yesno.wtf/assets/yes/14-b57c6dc03aa15a4b18f53eb50d6197ee.gif',
    }
]);

const onMessage = (text: string) => {
    messages.value.push({
        id: new Date().getTime(),
        itsMine: true,
        message: text,
    });
}

</script>

<template>
    <div class="bg-gray-100 h-screen flex flex-col max-w-lg mx-auto">
        <div class="bg-blue-500 p-4 text-white flex justify-between items-center">
            <span>Mi esposa</span>
        </div>

        <!-- Chat Messages -->
        <ChatMessages :messages="messages" />

        <!-- MessageBox -->
        <MessageBox @send-message="onMessage($event)" />


    </div>
</template>