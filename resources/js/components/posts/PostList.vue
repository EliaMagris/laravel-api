<template>
    <div>
        <ul v-if="posts.length">
            <li v-for="elem in posts" :key="elem.id">
                {{ elem.title }}
                <span v-if="elem.category">
                    {{ elem.category.name }}
                </span>
            </li>
        </ul>
        <p v-else>Non ci sono post nel DB</p>
    </div>
</template>

<script>

export default {
    name: 'PostList',
    components: {
        
    },
   
}
</script>

<style scoped lang="scss">
</style>