<template>
    <div>
        this is my message : {{message}}
    </div>
</template>
<script>
export default {
    props:[{'message' : String,}]
};
</script>