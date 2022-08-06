<template>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div className="body">
      <div className="top">
        <User :userData="tweet.user" />
      </div>
      <Timestamp :time="tweet.timestamp" />

      <Message :msg="tweet.message" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script>
import ProfileImage from "./ProfileImage.vue";
import Timestamp from "./Timestamp.vue";
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import User from "./User.vue";

export default {
  props: {
    tweet: Object
    // image: String,
    // userData: Object,
    // timestamp: String,
    // msg: String,
  },
  components: { 
    ProfileImage, 
    Timestamp, 
    Actions, 
    User, 
    Message
  },
};
</script>


<style scoped>
a {
  color: #42b983;
}
</style>