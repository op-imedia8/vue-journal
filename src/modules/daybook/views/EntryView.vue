<template>
  <div class="entry-title d-flex justify-content-between p2">
    <div>
        <span class="text-succes fs-3 fw-bold">15</span>
        <span class="mx-1 fs-3">octuber</span>
        <span class="mx-2 fs-4 fw-light">2021, jueves</span>
    </div>

    <div>
        <button class="btn btn-danger mx-2">Borrar
            <i class="fa fa-trash-alt"></i>
        </button>
        <button class="btn btn-primary">Subir Foto
            <i class="fa fa-upload"></i>
        </button>
    </div>
  </div>

  <hr>
  <div class="d-flex flex-column px-3 h-75">
    <textarea placeholder="Que sucedio hoy?"></textarea>
  </div>

  <Fab icono="fa-save"/>

  <img src="https://images.unsplash.com/photo-1557456170-0cf4f4d0d362?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80" alt="" class="thumbanil">
</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core'
export default {

    components:{
        Fab: defineAsyncComponent(()=> import('../components/Fab.vue'))
    }

}
</script>

<style lang="scss" scoped>
textarea{
    font-size: 20px;
    border:none;
    height: 100%;

    &:focus{
        outline:none;
    }
}

img{
    width:200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>