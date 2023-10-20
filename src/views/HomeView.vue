<template>
  <div>
    <section id="hero-section" class="mx-4 pt-10 mx-md-10">
      <Heading />
      <v-row class="pt-10">
        <v-col cols="12" md="8" class="pr-md-10">
          <p class="text-h2 font-weight-bold white--text">
            Connect, Consult, and Care Remotely
          </p>
        </v-col>
        <v-col cols="12" md="4" class="ml-auto">
          <p class="body-1 white--text">
            Get high-quality service with quality telemedecine. Take control of
            your health and experience the benefits of telemedecine with our
            platform
          </p>
          <div class="d-flex flex-row align-center pr-md-10">
            <v-btn rounded block class="mr-2 py-7 px-16" color="#9CC4E1"
              >Let's Talk!</v-btn
            >
            <v-btn fab><v-icon>mdi-play</v-icon></v-btn>
          </div>
        </v-col>
      </v-row>
      <v-img class="mt-auto d-none d-md-flex" src="../assets/Banner.png" height="460" contain></v-img>
      <v-img id="banner-button" class="d-none d-md-flex"  src="../assets/hero banner button.png" max-height="200" contain></v-img>
    </section>

    <section id="about-section">
      <AboutUs />
    </section>

    <v-img src="../assets/Slider.png" class="my-16"></v-img>

    <section id="steps-section" class="mx-4 mx-md-16 mb-10 px-md-16">
      <v-row class="mx-md-16">
        <v-col cols="12" md="6">
          <p class="text-h4 mb-6 text-center text-md-left">
            Pre-Clinical Intake That’s <br /><span
              >As Easy As Sending A Text</span
            >
          </p>
        </v-col>
        <v-col cols="12" md="6">
          <div class="d-flex flex-column flex-md-row justify-center">
            <v-spacer class="d-none d-md-flex"></v-spacer>
            <v-btn color="#9CC4E1" elevation="0" rounded class="py-7 px-16"
              >Learn More</v-btn
            >
          </div>
        </v-col>

        <v-container>
          <v-timeline class="mx-auto">
            <v-timeline-item>
              <v-card
                flat
                class="d-flex flex-column justify-start pa-5 card-steps"
                color="#0F152B"
              >
                <div>
                  <v-card-title class="text-h4 white--text">01</v-card-title>
                  <v-card-text class="pa-0">
                    <v-card-subtitle class="text-body-1 white--text"
                      >Pre-visit text serve as appointment reminders and
                      initiate patient intake</v-card-subtitle
                    >
                  </v-card-text>
                </div>
              </v-card>
            </v-timeline-item>

            <v-timeline-item>
              <v-card flat color="#0F152B" class="card-steps pa-5">
                <v-img src="../assets/Steps 1.png" contain max-width="200"></v-img>
              </v-card>
            </v-timeline-item>

            <v-timeline-item>
              <v-card
                flat
                class="d-flex flex-column justify-start pa-5 card-steps"
                color="#0F152B"
              >
                <div>
                  <v-card-title class="text-h4 white--text">02</v-card-title>
                  <v-card-text class="pa-0">
                    <v-card-subtitle class="text-body-1 white--text"
                      >Different experience for new and old
                      patients</v-card-subtitle
                    >
                  </v-card-text>
                </div>
              </v-card>
            </v-timeline-item>

            <v-timeline-item>
              <v-card
                flat
                class="d-flex flex-column justify-start pa-5 card-steps"
                color="#0F152B"
              >
                <div>
                  <v-card-title class="text-h4 white--text">03</v-card-title>
                  <v-card-text class="pa-0">
                    <v-card-subtitle class="text-body-1 white--text"
                      >Unique link opens an interactive with Health
                      Note</v-card-subtitle
                    >
                  </v-card-text>
                </div>
              </v-card>
            </v-timeline-item>

            <v-timeline-item>
              <v-card flat color="#0F152B" class="card-steps pa-5">
                <v-img src="../assets/Steps 4.png" contain max-width="200"></v-img>
              </v-card>
            </v-timeline-item>
          </v-timeline>
        </v-container>
        <!-- <v-col cols="12" md="4" v-for="(step, i) in steps">
          <v-card
            flat
            class="d-flex flex-column justify-start pa-5 mx-auto card-steps"
            color="#0F152B"
            height="300"
          >
            <div>
              <v-card-title class="text-h4 white--text">{{
                i + 1
              }}</v-card-title>
              <v-card-text>
                <v-card-subtitle class="text-body-1 white--text">{{
                  step.description
                }}</v-card-subtitle>
              </v-card-text>
            </div>
          </v-card>
        </v-col> -->
      </v-row>
    </section>

    <section id="client-testimonials">
      <v-img src="../assets/Testimonials Background.png" max-height="700">
        <h1 class="font-weight-bold text-center white--text mt-10 mb-8">
          Client Testimonials
        </h1>

        <v-carousel class="px-4">
          <v-carousel-item
            v-for="(client, i) in clients"
            :key="i"
            reverse-transition="fade-transition"
            transition="fade-transition"
          >
            <v-card flat class="cards mx-auto pa-10" max-width="700">
              <v-img
                contain
                max-width="100"
                class="mx-auto"
                src="../assets/Testimonial Separate 2.png"
              ></v-img>
              <v-card-title class="text-h3 d-flex justify-center">{{
                client.name
              }}</v-card-title>
              <v-card-subtitle class="text-subtitle-2 text-center"
                >{{ client.age }} years old</v-card-subtitle
              >
              <v-card-text class="text-center">{{
                client.testimonial
              }}</v-card-text>
            </v-card></v-carousel-item
          >
        </v-carousel>
      </v-img>
    </section>

    <section id="article-section" class="pt-10 mx-4 px-md-16 mx-md-16">
      <p class="text-h4">Not just words, Take a look at our writing.</p>

      <v-divider></v-divider>
      <div class="d-flex flex-column flex-md-row align-md-center my-8">
        <p class="text-body-1 mr-4">
          Reading a book is a silent conversation between you and the author.
          <br />Hesitating to join? Start with out writing. it will help you
          calm down.
        </p>
        <v-spacer></v-spacer>
        <v-btn rounded class="mr-2 py-7 px-16" color="#9CC4E1"
          >Let's Talk!</v-btn
        >
      </div>

      <v-divider></v-divider>

      <v-row class="mt-10">
        <v-col cols="12" md="4" v-for="(article, i) in articles">
          <v-card
            flat
            class="d-flex flex-column justify-space-between pa-5 mx-auto card-steps"
            :color="article.color"
            height="500"
          >
            <v-card flat class="article-headline-container">
              <div class="d-flex align-center">
                <v-chip class="ma-2" color="primary">
                  {{ article.topic }}
                </v-chip>
                <p class="text-overline pa-0 mb-0 white--text">
                  {{ article.date }}
                </p>
              </div>
              <v-card-title class="text-h4 white--text">{{
                article.headline
              }}</v-card-title>
            </v-card>
            <v-card-text class="px-0">
              <v-card-subtitle class="text-body-1 white--text">{{
                article.content
              }}</v-card-subtitle>
            </v-card-text>
            <v-card-actions class="mt-auto">
              <v-btn rounded outlined block class="white--text"
                >Read More</v-btn
              >
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </section>

    <section id="footer-section" class="pt-10 mt-10 mx-10">
      <v-row class="pt-10">
        <v-col cols="12" md="8" class="pr-md-10">
          <p class="text-h2 font-weight-bold white--text">
            Connect, Consult, and Care Remotely
          </p>
        </v-col>
        <v-col cols="12" md="4" class="ml-auto">
          <p class="body-1 white--text">
            Get high-quality service with quality telemedecine. Take control of
            your health and experience the benefits of telemedecine with our
            platform
          </p>
          <div class="d-flex flex-row align-center pr-md-10">
            <v-btn rounded block class="mr-2 py-7 px-16" color="#9CC4E1"
              >Let's Talk!</v-btn
            >
            <v-btn fab><v-icon>mdi-play</v-icon></v-btn>
          </div>
        </v-col>
      </v-row>
      <Heading class="mt-10" />
    </section>
  </div>
</template>

<script>
import Heading from "../components/LandingPage/Heading";
import HeroSection from "../components/LandingPage/HeroSection";
import PageContent from "../components/LandingPage/PageContent";
import Testimonials from "../components/LandingPage/Testimonials";
import AboutUs from "../components/LandingPage/AboutUs";

export default {
  name: "Home",
  components: {
    Heading,
    HeroSection,
    PageContent,
    Testimonials,
    AboutUs,
  },

  data: () => ({
    clients: [
      {
        name: "Justin Austin",
        age: 43,
        testimonial:
          " Feel better. The mentor listened very well, felt very understanding because what I felt was validated by the mentor that it was normal. Was given advice from different points of view which I thought was great.",
      },
      {
        name: "Prince Charles Clemente",
        age: 47,
        testimonial:
          " Feel better. The mentor listened very well, felt very understanding because what I felt was validated by the mentor that it was normal. Was given advice from different points of view which I thought was great.",
      },
      {
        name: "Gabriel Gatbonton",
        age: 42,
        testimonial:
          " Feel better. The mentor listened very well, felt very understanding because what I felt was validated by the mentor that it was normal. Was given advice from different points of view which I thought was great.",
      },
    ],

    steps: [
      {
        image: "Steps 1.png",
        description:
          "Pre-visit text serve as appointment reminders and initiate patient intake",
      },
      {
        image: "Steps 4.png",
        description: "Different experience for new and old patients",
      },
      {
        image: "Steps 4.png",
        description: "Unique link opens an interactive with Health Note",
      },
    ],

    articles: [
      {
        color: "#5A6282",
        headline:
          "Heavy Stress? Come On, Identify The Causes And How To Overcome Them!",
        topic: "Mental Health",
        date: "2023, 25 May",
        content:
          "Lorem ipsum dolor sit amet consectetur. Imperdiet id nunc eu tincidunt at in facilisis. Nibh vitae consequat elit varius aliquam aliquam quis lectus.",
      },
      {
        color: "#0F152B",
        headline:
          "Often Blame others When Failed? Recognize Self-Serving Bias Behavior",
        topic: "Self Understanding",
        date: "2023, 13 June",
        content:
          "Lorem ipsum dolor sit amet consectetur. Imperdiet id nunc eu tincidunt at in facilisis. Nibh vitae consequat elit varius aliquam aliquam quis lectus.",
      },
      {
        color: "#3E92B6",
        headline: "7 Signs Your Mental Health Is In Good Condition",
        topic: "Mental Health",
        date: "2023, 25 May",
        content:
          "Lorem ipsum dolor sit amet consectetur. Imperdiet id nunc eu tincidunt at in facilisis. Nibh vitae consequat elit varius aliquam aliquam quis lectus.",
      },
    ],
  }),
};
</script>

<style scoped>
#hero-section {
  background-color: #0f152b;
  height: 100vh;
  border-radius: 0 0 100px 100px;
  padding-left: 100px;
  padding-right: 100px;
}

#banner-button{
  margin-top: -50px;
}

span {
  color: #3e92b6;
}

@media screen and (min-width: 480px) {
  #hero-section {
    background-color: #0f152b;
    height: 100vh;
    border-radius: 0 0 100px 100px;
  }
}

/* ABOUT SECTION ######################## */
#about-section {
  display: flex;
  justify-content: center;
  margin-top: 50px;
}

/* STEPS SECTION ######################## */

.card-steps {
  border-radius: 50px;
}

/* TESTIMONIALS ######################### */
#client-testimonials h1 {
  font-size: 3rem;
}

.cards {
  border-top-left-radius: 50px;
  border-bottom-right-radius: 50px;
}

/* ARTICLES ############################ */
.article-headline-container {
  height: 50%;
  background-color: transparent;
}

/* FOOTER ############################## */
#footer-section {
  background-color: #0f152b;
  border-radius: 100px 100px 0 0;
  padding-left: 100px;
  padding-right: 100px;
}
</style>
