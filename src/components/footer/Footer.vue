<template>
  <div class="container">
    <div class="container-1">
    <div class="top-part">
      <img src="../../assets/logos/martineli-ginetto.logo.svg"/>
      <div class="top-right">
        <a class="top-right-item contacti">contacti</a>
        <img class="instagram top-right-item" src="../../assets/logos/instagram.logo.svg"/>
        <img class="facebook top-right-item" src="../../assets/logos/facebook.logo.svg"/>
      </div>
    </div>
    <div class="services">
      <div class="services-description">
        Dal 1947 lo spirito imprenditoriale <strong>MARTINELLIGINETTO</strong> si fonda sulle competenze tecniche, 
        l’utilizzo delle tecnologie tessili più avanzate e sulla capacità di mobilitare energie 
        professionali e creative in grado di innovare il prodotto a tutti i livelli.
      </div>
      <Services :key="service" v-for="service in services" :service="service" />
    </div>
    <div class="separator" />
    <Clients/>
    <div class="separator" />
    <div class="footer-bottom-part">
      <div>
        <a class="link privacy">Privacy</a>
        <a class="link cookie">Cookie policy</a>
      </div>
      <div>Martinelli Ginetto S.p.A - C.F. e Partita Iva 03403660164 Cap.Sociale 10.000.000 I.v. REA: BG – 375519</div>
    </div>
  </div>
  </div>
</template>

<script>
import Services from '@/components/footer/Services.vue';
import Clients from '@/components/footer/Clients.vue'
export default {
  name: "Footer",
  components: {
    Services,
    Clients
  },
  data: () => ({services: [
    {
    title: 'SETTORI',
    contents: ['Filati', 'Tessuti', 'Nobilitazione', 'Editoria']
    },
    {
    title: 'INNOVAZIONE',
    contents: ['Creatività e Design', 'Realtà produttiva', 'Vision Digitale']
    },
    {
    title: 'Responsabilità',
    contents: ['Economica', 'Ambientale', 'Sociale']
    },
    {
    title: 'CARRIERA',
    contents: ['Giovani', 'Scuola lavoro', 'Lavora con noi']
    }
]})
}
</script>

<style scoped>
  .instagram {
    fill: #FFFFFF;
  }

  .facebook {
    fill: #FFFFFF;
  }

  .top-part {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .container {
    background-color: #1E1E1E;
    color: #FFFFFF;
  }

  .container-1 {
    width: 85%;
    margin: auto;
    padding-top: 4rem;
  }

  .top-right {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .top-right-item {
    padding: 10px;
  }

  .contacti {
    text-decoration: underline;
  }

  .services {
    display: flex;
    justify-content: space-between;
    padding-top: 32px;
  }

  .services-description {
    flex-basis: 20%;
    font-size: 12px;
    line-height: 20px;
    padding: 5px;
  }

  .separator {
    width: 100%;
    height: 2px;
    background-color: rgba(255, 255, 255, 0.3);
  }

  .footer-bottom-part {
    display: flex;
    justify-content: space-between;
    padding: 2rem 0rem;
    opacity: 0.8;
    font-size: 11px;
    line-height: 28px;
    font-weight: 400;
  }
  .link {
    text-decoration: underline;
  }

  .cookie {
    padding-left: 2rem;
  }
</style>