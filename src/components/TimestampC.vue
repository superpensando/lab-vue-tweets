<template>
  <span className="timestamp">{{ timeStamp }}</span>
</template>

<script>
export default {
  name: 'TimestampC',
  props: {
    timeStamp: String,
  },
}

</script>