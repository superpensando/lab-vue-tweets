<template>
   <p className="message">
        {{ message }}
    </p>
</template>

<script>
export default {    
    name: 'MessageC',
     props: {
         message: String,
    },
}
   
</script>