<script setup>
    import Input from './Input.vue'
    import Button from './Button.vue'
    import TodoList from './TodoList.vue'
    import IconArrowUp from './icons/IconArrowUp.vue'
</script>

<template>
    <div class="todo" >
        <div class="todo-header">
            <Input :placeholder="`Add item...`"/>
            <Button />
        </div>
        <TodoList/>
        <div class="scroll-to-top">
            <a @click="scrollToTop">
                <IconArrowUp/>
            </a>
        </div>
    </div>
</template>

<style scoped>
  .todo {
    position: relative;
    font-size: 18px;
  }

  .todo-header {
    display: flex;
    padding: 50px 40px 50px 40px;
  }

  .scroll-to-top {
    display: flex;
    justify-content: center;
    margin-top: 20px;
  }

  .scroll-to-top a {
    background-color: #15A381;
    border-radius: 50%;
    height: 44px;
    width: 44px;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
  }

  .scroll-to-top a:hover {
        cursor: pointer;
        background-color: #208f74;
    }

</style>