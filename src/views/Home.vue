<template>
    <div class="home">esto es una prueba</div>
    <Header/>
    <Modal :modalActive="modalActive" @close="toggleModal">
        <div class="modal-content">
            <h1>This is a Modal header</h1>
            <p>This is a message</p>
        </div>
    </Modal>
    <button @click="toggleModal" type="button"> Open Modal</button>
</template>

<script>
import Modal from "../components/Modal.vue";
import Header from "../components/Header.vue";
import { ref } from 'vue';
export default {
    name: "Home",
    components: {
        Modal,
        Header
    },
    setup() {
        const modalActive= ref(false);

        const toggleModal =() =>{
            modalActive.value = !modalActive.value;
        }

        return {
            modalActive,
            toggleModal
        };
    }
}


</script>