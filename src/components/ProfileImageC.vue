<template>
   <img
      className="profile"
      alt="profile"
      :src="ProfileImageSrc"
    />
</template>

<script>
export default {    
    name: 'ProfileImageC',
     props: {
         ProfileImageSrc: String,
    },
}
   
</script>