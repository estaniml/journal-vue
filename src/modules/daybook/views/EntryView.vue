<template>
  <div>

    <div>
        <span>15 </span>
        <span>Mayo </span>
        <span>2023</span>
    </div>

    <div class="btn-container">
        <button class="delete-btn">
            borrar
        </button>
        
        <button class="upload-btn">
            subir foto
        </button>
    </div>
  </div>

  <hr>

  <div>
    <textarea placeholder="aosjkdao aosdj as"></textarea>
  </div>

  <FabBtn />

    <img 
        src="https://images.unsplash.com/photo-1683130461782-2a3f1910da18?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1169&q=80" 
        alt="" 
    />


</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
    components: {
        FabBtn: defineAsyncComponent(() => import('../components/FabBtn.vue'))
    }
}
</script>

<style lang="scss" scoped>
    textarea {
        font-size: 16px;
        border: none;
        height: 100%;
        width: 100%;
        resize: none;
        
        &:focus {
            outline: none;
        }
    }

    img{
        width: 100%;
        margin: 0 auto;
        box-shadow: 2px 4px 20px #2c2c2c;
    }

    .btn-container button {
        padding: 10px 20px;
        text-transform: uppercase;
        font-weight: 600;
        font-size: 12px;
        border: none;
        border-radius: 5px;
        color: #fff;
        cursor: pointer;
        box-shadow: 1px 1px 5px #121212;

        &:hover{
            filter: brightness(1.2);
            box-shadow: 1px 1px 10px #191818;
        }
    }

    .btn-container{
        display: flex;
        gap: 1rem;
        margin: 10px auto;
    }

    .delete-btn{
        background-color: rgb(245, 56, 56);
    }

    .upload-btn{
        background-color: rgb(56, 81, 245);
    }
</style>