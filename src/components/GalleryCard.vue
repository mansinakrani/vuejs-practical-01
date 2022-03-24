<template>
    <div class="container">
      <h1>{{ title }}</h1>
      <h3>{{ heading }}</h3>
      <img src="https://images.unsplash.com/photo-1590362891991-f776e747a588?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTN8fGNhciUyMGRlYWxlcnxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=800&q=60" alt="Mercedes Car" />
      <h4>{{ details }}</h4>
      <button type="button" @click="info">Info</button>
    </div>
</template>

<script>
export default {
  name: 'GalleryCard',
  data() {
    return {
      title: "Car Showroom",
      heading: "MERCEDES-BENZ GLC COUPE",
      details: "Mercedes-Benz GLC Coupe is offered in 2 variants - the base model of GLC Coupe is 300 4MATIC is the petrol variant in the GLC Coupe lineup and is priced at ₹ 70.95 Lakh and the top variant Mercedes-Benz GLC Coupe 300d 4MATIC which comes at a price tag of Rs. 72.00 Lakh",
    };
  },
  methods: {
  info() {
    alert(`Car Price is ₹ 70-73 Lakh !`)
  }
}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container{
 background-color: rgb(187, 234, 235);
 border-radius: 15px;
 box-shadow: rgba(112, 112, 220, 0.1) 0px 8px 24px, rgba(223, 28, 28, 0.1) 0px 16px 56px, #f265651a 0px 24px 80px;
}

h1 {
  text-shadow: 5px 5px 5px rgb(103, 126, 128);
}

h3 {
  margin: 20px 0 0;
  font-style: oblique;
}

img {
  height: 350px;
  width: auto;
}

h4 {
  font-size: medium;
}

button {
  align-items: center;
  background-image: linear-gradient(144deg,#88aee8, #deb5b5 50%,#00DDEB);
  border: 0;
  border-radius: 8px;
  box-shadow: rgba(151, 65, 252, 0.2) 0 15px 30px -5px;
  box-sizing: border-box;
  color: #ffffff;
  font-family: Phantomsans, sans-serif;
  font-size: 20px;
  justify-content: center;
  line-height: 1em;
  max-width: 100%;
  min-width: 140px;
  padding: 15px 20px;
  text-decoration: none;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  white-space: nowrap;
  cursor: pointer;
  margin-block-end: 8px;
}

.button:active,
.button:hover {
  outline: 0;
}

@media (min-width: 768px) {
  .button {
    font-size: 24px;
    min-width: 196px;
  }
}

@media (max-width: 300px) {
  img {
    height: 100px;
    width: 150px;
  }
}

@media (max-width: 700px) {
  img {
    height: 150px;
    width: 250px;
  }

  h1 {
    font-size: 29px;
  }

  h3 {
    margin: 20px 0 0;
    font-style: oblique;
    font-size: 20px;
  }

  h4 {
    font-size: small;
  }
}
</style>
