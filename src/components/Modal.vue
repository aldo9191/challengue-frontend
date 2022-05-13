<template>
    <transition name="modal-animation">
        <div v-show="modalActive" class="modal">
            <transition name="modal-animation-inner">
             <div v-show="modalActive" class="modal-inner">
                
                <!-- Modal Content-->
                <i @click="close" class="fa-solid fa-circle-xmark"></i>
                <slot />
                <button @click="close" type="button">Close </button>
             </div>
            </transition>
        </div>
    </transition>
</template>

<script>
export default {
    props: ["modalActive"],
    setup(props, { emit }){
        const close = () => {
            emit("close")
        }
    return {close}
    }
}
</script>

<style></style>