<template>
  <div className="tweet">
    <img
      className="profile"
      alt="profile"
      :src="tweet.user.image"
    />

    <div className="body">
      <div className="top">
        <span className="user">
          <span className="name">{{ tweet.user.name }}</span>
          <span className="handle">{{ tweet.user.handle}}</span>
        </span>

        <span className="timestamp">{{ tweet.timeStamp }}</span>
      </div>

      <p className="message">
        {{ tweet.message }}
      </p>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
export default {
    name: 'TweetC',
    props: {
        tweet:Object
    },
}
</script>

<style lang="scss">
  a {
    color: #42b983;
  }
</style>