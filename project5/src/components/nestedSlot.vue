<template>
    <div>
        <slot name="parent-slot">
            <slot name="child-slot">
                <slot name="grand-child-slot"></slot>
            </slot>
        </slot>
        <nested-head>
            <slot name="slot1"></slot>
            <slot name="slot2"></slot> 
        </nested-head>
    </div>
</template>

<script>
export default {
    
    
}
</script>

<style scoped>

</style>