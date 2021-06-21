<template>
    <li :class="attivo()">
        {{text}}
    </li>
</template>

<script>
export default {
    name: 'LinkMenu',
    props: {
        text: String,
        link: String,
        active: Boolean
    },
    methods: {
        attivo: function() {
            if (this.active) {
                return "active"
            } else {
                return ""
            }
        }
    }
}
</script>

<style scoped lang="scss">
li {
    margin-left: 20px;
    color: #5b2ca2;
    padding-bottom: 5px;
}
.active {
    border-bottom: 3px solid #5b2ca2;
}
</style>