<template>
    <div class="modals">
        <h1>Modals</h1>
        <button @click="showModal = true ">Show Modal</button>
        <Modal v-if="showModal"><p>Lorem ipsum dolor sit amet consectetur adipiscing</p>
        </Modal>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import Modal from '@/components/Modal.vue'

const showModal = ref(true)
</script>

<!--
<script>
import Modal from '@/components/Modal.vue'

export default {
    components: {
        Modal
    }
}

</script>
-->