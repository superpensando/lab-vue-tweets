<template>
 <span className="user">
   <span className="name">{{ name }}</span>
   <span className="handle">{{ handle }}</span>
</span>
</template>

<script>
export default {
 name: 'UserC',
     props: {
         name: String,
         handle:String,
    },
}
</script>