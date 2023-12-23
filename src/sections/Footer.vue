<template>
  <section>
    <div class="container">
      <footer class="py-5">
        <div class="row">

          <template v-for="section in footer_section" :key="section.title">
            <div class="col-2">
            <h5 class="text-uppercase">{{section.title}}</h5>
            <img src="@/assets/images/Divider.svg" width="60" class="mb-3"/>
            <ul class="nav flex-column">
              <li class="nav-item mb-2" v-for="item in section.items" :key="item.title">
                <a :href="item.link" class="nav-link p-0">{{ item.title }}</a>
              </li>
            </ul>
          </div>
          </template>
          
          <div class="col-2 offset-1">
            <h5 class="text-uppercase">Follow Us</h5>
            <img src="@/assets/images/Divider.svg" width="60" class="mb-3"/>
            
            <p>
              <a href="" class="mr-4"> <img src="@/assets/images/instagram.svg" class="social-image"></a>
              <a href="" class="mr-4"> <img src="@/assets/images/facebook.svg" class="social-image"></a>
              <a href="" class="mr-4"> <img src="@/assets/images/twitter.svg" class="social-image"></a>
            </p>
          </div>
        </div>

        <div class="py-4 mt-5">
          <p class="text-center">
            Copyright © Night Trips 2019. All rights reserved.
          </p>
          <p class="text-center section-title">NT.</p>
        </div>
      </footer>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      footer_section: [
        {
          title: "About",
          items: [
            {
              title: "Our Mission",
              link: "/missions",
            },
            {
              title: "Terms",
              link: "/terms",
            },
            {
              title: "Copyright",
              link: "/copyright",
            },
          ],
        },

        {
          title: "Faq",
          items: [
            {
              title: "Rules",
              link: "/rules",
            },
            {
              title: "Tickets",
              link: "/tickets",
            },
            {
              title: "Editions",
              link: "/editions",
            },
            {
              title: "Contribute",
              link: "/contribution",
            },
          ],
        },
        {
          title: "Events",
          items: [
            {
              title: "Star Gazing",
              link: "/events",
            },
            {
              title: "Desset Mania",
              link: "/events",
            },
            {
              title: "DUne Madness",
              link: "/events",
            },
            {
              title: "Spooky Land",
              link: "/events",
            },
          ],
        },

        {
          title: "Contact Us",
          items: [
            {
              title: "hello@example.com",
              link: "email:hello@example.com",
            },
            {
              title: "(405) 555-0128",
              link: "tel:(405) 555-0128",
            },
            {
              title: "(252) 555-0126",
              link: "tel:(252) 555-0126",
            },
            
          ],
        },
      ],
    };
  },
};
</script>

<style scoped>
.footer-title-list {
  margin-bottom: 10px;
}

footer h5 {
  padding-bottom: 10px;
}

footer .nav-item a {
  text-decoration: none;
  color: #fff;
}

footer .nav-item {
  margin-bottom: 10px;
}

.social-image{
  width: 30px;
  height: 30px;
  margin-right: 15px;
}
</style>
