<template>
  <div>
    <Hero />
    <div class="information">
      <h1>All chart types available anywhere you code</h1>
      <h3>The largest set of charts and graphs available in the market.</h3>
      <h5>
        Pick from our library of custom-crafted charts or create your own.
        Manage your visualizations directly within your project to ensure graphs
        and charts look great and stay on brand.
      </h5>
      <div class="information__button">
        <v-btn depressed color="primary" height="50px">
          View all charts
          <v-icon right color="white"> mdi-arrow-right </v-icon>
        </v-btn>
      </div>
    </div>
    <div class="information">
      <h1 data-aos="fade-up">
        Advanced features for developers focused on Business Intelligence
      </h1>
      <h3 data-aos="fade-up" data-aos-delay="50">
        A myriad of Business Intelligence and Data Visualization development
        tools available for instant download.
      </h3>
    </div>
    <div class="information">
      <v-container-fluid>
        <v-row>
          <v-col
            cols="12"
            sm="6"
            v-for="card in cardData"
            :key="card.title"
            data-aos="fade-up"
            data-aos-delay="100"
          >
            <Card
              :img="card.img"
              :title="card.title"
              :text="card.text"
              :subtitle="card.subtitle"
              :icon="card.icon"
            />
          </v-col>
        </v-row>
      </v-container-fluid>
    </div>
    <Footer />
  </div>
</template>

<script>
import aosMixin from '~/mixins/aos'

export default {
  name: 'Index',
  mixins: [aosMixin],
  data() {
    return {
      cardData: [
        {
          img: require('@/assets/images/hierarchy.svg'),
          title: 'Easy integration to MVC applications',
          text: "Chart FX provides developers advanced charting features with minimal integration effort. Helpful tools like the Chart Wizard, Tutorial and Samples Resource and a Programmer's Guide will assist you in creating visually impressive data visualization solutions with little time invested.",
        },
        {
          img: require('@/assets/images/thermostat.svg'),
          title: 'Data Analysis',
          text: "Chart FX provides end-user chart customization through intuitive menus, dialogs and toolbars. Through its enhanced interface, users can export the charts to a variety of formats, as well as store changes to a particular chart for future sessions, maximizing the usability and readability of your application's charts at the end-user level.",
        },
        {
          img: require('@/assets/images/visual-studio-icon-content.svg'),
          title: 'Seamless Visual Studio Integration',
          text: "Chart FX takes advantage of the .NET Framework to provide robust features. Within Visual Studio, we've been able to make the design-time experience not only more enjoyable, but more productive as well. By extending the smart tags to include a full wizard, it is now easier to achieve a more polished and finished look through a graphical interface with less need to write code.",
        },
        {
          img: require('@/assets/images/object.svg'),
          title: 'Advanced Graphics Capabilities',
          text: "To provide the greatest aesthetics for our tools, we make great use of .NET's GDI+ technology. Chart FX makes use of it extensively for much of the drawing and text in the various chart types.",
        },
        {
          img: require('@/assets/images/server.svg'),
          title: 'Effortless and Flexible Data Connectivity',
          text: "In both Chart FX and Grid FX, the data is what's important. Both allow you to connect to data sources through ADO.NET and create business objects connections for easier development. Chart FX also adds the ability to accept data from an XML file.",
        },
        {
          img: require('@/assets/images/server.svg'),
          title: 'Documentation and Samples at hand!',
          text: 'We deliver a comprehensive Documentation with a wealth of actual samples (and code) that you can integrate and test in your applications. A single repository for Chart FX documentation without any duplication.',
          subtitle: 'View the documentation',
          icon: 'mdi-arrow-right',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.information {
  background-color: #ebebeb;
  padding-top: 50px;
  padding-left: 40px;
  padding-right: 40px;

  h1 {
    text-align: center;
    font-size: 50px;
    font-family: 'Graphik Semibold', Fallback, sans-serif;
    color: #000;
  }

  h3 {
    text-align: center;
    font-size: 30px;
    font-family: 'Graphik Medium', Fallback, sans-serif;
    color: #000;
    padding-top: 20px;
  }

  h5 {
    text-align: center;
    justify-content: center;
    font-family: 'Graphik Light', Fallback, sans-serif;
    color: #000;
    font-size: 20px;
    padding-top: 20px;
    padding-left: 30px;
    padding-right: 30px;
  }

  &__button {
    display: flex;
    justify-content: center;
    padding-top: 30px;
    padding-bottom: 80px;
  }
}
</style>
