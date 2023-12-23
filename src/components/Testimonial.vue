<template>
  <div class="col-md-6">
    <div class="testimonial-card p-5 mb-4">
      <div class="testimonial-content">
        <img
          src="@/assets/images/testimonial.svg"
          width="30"
          height="30"
          class="testimonial-icon"
        />
        <p class="font-weight-bold">
          {{ testimonial.title }}
        </p>

        <p>
            {{ testimonial.content }}
        </p>

        <div class="author">
          <img :src="testimonial.user_image" class="author-image" />
          <div class="author-details">
            <p>{{ testimonial.user_name }}</p>
            <p>{{ testimonial.user_job }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["testimonial"],
};
</script>

<style scoped>
.testimonial-card {
  background: #02223b;
  border-radius: 8px;
}

.testimonial-content {
  position: relative;
  padding-left: 45px;
  line-height: 27px;
}
.testimonial-icon {
  position: absolute;
  top: 0;
  left: 0;
}

.author {
  margin-top: 40px;
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}
.author-image {
  width: 80px;
  height: 80px;
  object-position: center;
  object-fit: cover;
}

.author-details {
    margin-left: 20px;
  font-size: 15px;
  line-height: 20px;
  font-weight: bold;
}
</style>
