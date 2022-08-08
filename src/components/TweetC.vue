<template>
  <div className="tweet">

    <ProfileImageC :ProfileImageSrc="tweet.user.image" />

    <div className="body">
      <div className="top">

        <UserC :name="tweet.user.name" :handle="tweet.user.handle" />

        <TimestampC :timeStamp="tweet.timestamp" />

      </div>

      <MessageC :message="tweet.message" />

      <ActionsC />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImageC from './ProfileImageC.vue';
import TimestampC from './TimestampC.vue';
import MessageC from './MessageC.vue';
import UserC from './UserC.vue';
import ActionsC from './ActionsC.vue';

export default {
  name: "TweetC",
  props: {
    tweet: Object
  },
  components: { TimestampC, MessageC, ProfileImageC, UserC, ActionsC }
}

</script>

<style lang="scss">
a {
  color: #42b983;
}
</style>