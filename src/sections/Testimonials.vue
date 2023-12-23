<template>
  <section class="section">
    <BlurPoint width="500" top="0" right="70" background_color="#41EAD4" />
    <BlurPoint width="500" top="450" right="70" background_color="#BE41EA" />
    <BlurPoint width="200" top="450" right="70" background_color="#7741EA" />

    <BlurPoint width="500" left="0" right="70" background_color="#41EAD4" />
    <BlurPoint width="500" left="450" right="70" background_color="#BE41EA" />

    <div class="container">
      <div class="container-tests">
        <h1 class="section-title text-center mb-4">People’s thoughts</h1>
        <p class="section-subtitle text-center">SEE WHAT ARE OTHERS SAYING</p>

        <div class="row mt-5">
          <Testimonial
            v-for="testimonial in testimonials"
            :key="testimonial.id"
            :testimonial="testimonial"
          ></Testimonial>
        </div>

        <div class="mt-100 mb-100">
          <h1 class="section-title text-center mb-4">See you soon !</h1>
          <p class="section-subtitle text-center">
            We hope to meet each other very soon.
          </p>
        </div>
      </div>

      <div class="line"></div>
    </div>
  </section>
</template>

<script>
import Testimonial from "@/components/Testimonial.vue";
import BlurPoint from "@/components/BlurPoint.vue";
export default {
  components: { Testimonial, BlurPoint },
  data() {
    return {
      testimonials: [
        {
          id: 1,
          title: "Lorem ipsum dolor sit amet, consectetur adipisicing elit.",
          content:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium eos nulla aliquam eius sequi, cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet. cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet.",
          user_image: "images/author.jpg",
          user_name: "Judy ROSELESS",
          user_job: "MARKETING HEAD at ROM 2.",
        },
        {
          id: 2,
          title: "Lorem ipsum dolor sit amet, consectetur adipisicing elit.",
          content:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium eos nulla aliquam eius sequi, cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet. cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet.",
          user_image: "images/author.jpg",
          user_name: "Judy ROSELESS",
          user_job: "MARKETING HEAD at ROM 2.",
        },
        {
          id: 3,
          title: "Lorem ipsum dolor sit amet, consectetur adipisicing elit.",
          content:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium eos nulla aliquam eius sequi, cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet. cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet.",
          user_image: "images/author.jpg",
          user_name: "Judy ROSELESS",
          user_job: "MARKETING HEAD at ROM 2.",
        },
        {
          id: 4,
          title: "Lorem ipsum dolor sit amet, consectetur adipisicing elit.",
          content:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium eos nulla aliquam eius sequi, cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet. cumque vero molestiae neque! Nobis odit cumque amet ut sed, itaque voluptate aliquid neque laboriosam eveniet.",
          user_image: "images/author.jpg",
          user_name: "Judy ROSELESS",
          user_job: "MARKETING HEAD at ROM 2.",
        },
      ],
    };
  },
};
</script>

<style scoped>
.line {
  width: 2px;
  margin: auto;
  height: 80px;
  border-radius: 13px;
  border-radius: 13px;
  background: linear-gradient(180deg, #09f4f4 0%, #00c9e0 100%);
}

.container-tests{
  background: #011627;
  padding: 70px;
}
</style>
