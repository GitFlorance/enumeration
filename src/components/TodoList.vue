<template>
    <div>
        <ul>
            {{todos}}
            <TodoItem />
        </ul>
    </div>
</template>

<script>
import TodoItem from './TodoItem'

export default {
    props: ['todos'],
    components: {
    TodoItem
  }
}
</script>