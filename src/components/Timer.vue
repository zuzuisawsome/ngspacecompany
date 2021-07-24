<template>
    <span>{{ seconds }}</span>
</template>

<script>
export default {

    props: [ 'value' ],

    computed: {
    
        seconds: function() {
            return new Date(0, 0, 0, 0, 0, this.value).toTimeString().split(' ')[0]
        },
    },
}
</script>