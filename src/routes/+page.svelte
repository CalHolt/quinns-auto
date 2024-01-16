<script>
  import Nav from "../lib/components/Nav.svelte";
  import Footer from "../lib/components/Footer.svelte";
</script>
<Nav />
<!-- Hero Section -->

<div class="image p-10">
<div class="hero flex-col sm:flex-row flex justify-center items-center gap-20 p-5">
  <div class="flex flex-cols text-center text-5xl md:text-7xl gap-4">
    <h1>Quinn's Auto Service</h1>
  </div>
  <div class="flex flex-col justify-center max-w-80 sm:content-center text-center text-xl">
    <span>We offer quality auto repairs backed by years of experience!</span>
    <a class="my-5" href="tel:4032423038"><button>Call Now</button></a>
    <span class="">(403) 242-30338 / (825) 540-1256</span>
  </div>
</div>
</div>

<!-- Services Section -->

<h2 class="text-center text-4xl p-4 services">Services</h2>
<div class="grid md:grid-cols-3 p-4 gap-6">
  <div class="flex flex-col p-4 card items-center justify-center service-card">
    <h4 class="text-2xl text-center">-Inspections-</h4>
    <ul class="list-disc my-8">
      <li>Out of Province</li>
      <li>Pre-Purchase</li>
      <li>Insurance</li>
      <li>AMVIC</li>
      <li>48 Point</li>
    </ul>
  </div>
  <div class="flex flex-col p-4 card items-center justify-center service-card">
    <h4 class="text-2xl text-center">-Routine Service-</h4>
    <ul class="list-disc my-8 ">
      <li>Oil Changes</li>
      <li>Alignments</li>
      <li>Tire Mount and Balance</li>
      <li>Fluid Flushes</li>
      <li>A/C Recharge</li>
    </ul>
  </div>
  <div class="flex flex-col p-4 card items-center justify-center service-card">
    <h4 class="text-2xl text-center">-Repairs-</h4>
    <ul class="list-disc my-8 ">
      <li>Brake Service</li>
      <li>Suspension / Steering</li>
      <li>Accident Damage Assesment</li>
      <li>Tire Repairs</li>
      <li>Fluid Leaks</li>
    </ul>
  </div>
</div>

<!-- Contact Section -->

<div class="flex flex-col md:flex-row justify-around p-2 items-center">
  <div class="p-5">
    <h3 class="py-5 text-3xl">Contact Us</h3>
    <p class="text-lg">Address: 3401 Spruce Drive SW</p>
    <p class="text-lg">Phone: (403) 242-3038</p>
    <p class="text-lg">E-Mail: qasltd01@gmail.com</p>

    <h3 class="py-5 text-3xl">Hours</h3>
    <ul>
      <li class="text-lg">Monday - Friday: 8am - 5pm</li>
      <li class="text-lg">Weekends: Closed</li>
      <li class="text-lg">Holidays: Closed</li>
    </ul>
  </div>
    
  <iframe class="py-5 px-2" title="Quinns Auto Service Maps" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d10033.011143372429!2d-114.14633816491535!3d51.04842003898797!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x53716e35d8514391%3A0x630279686330677!2sQuinn&#39;s%20Auto%20Service%20Ltd.!5e0!3m2!1sen!2sca!4v1704837594710!5m2!1sen!2sca" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
</div>

<!-- Footer -->

<Footer />
<style>
  .image {
    background-image: url($images/pexels-daniel-andraski-13065696.jpg);
    background-size: cover;
    background-position:25% 75%;
    background-repeat: no-repeat;
  }
  .hero {
    height: 65vh;
    /* From https://css.glass */
background: rgba(255, 255, 255, 0.58);
background-size: 10rem 15rem;
box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
backdrop-filter: blur(4.7px);
-webkit-backdrop-filter: blur(8.7px);
  }
  button {
  padding: 1.3em 3em;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 2.5px;
  font-weight: 500;
  color: #000;
  background-color: #fff;
  border: none;
  border-radius: 45px;
  box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease 0s;
  cursor: pointer;
  outline: none;
}

button:hover {
  background-color: #273fff;
  box-shadow: 0px 15px 20px #021eef;
  color: #fff;
  transform: translateY(-7px);
}

button:active {
  transform: translateY(-1px);
}

.card {
  height: 20rem;
}

.service-card {
  border: 2px solid white;
  transition: 0.5s ease-out;
}
/*Hover*/
.service-card:hover {
 border-color: #273fff;
 box-shadow: 0 4px 18px 0 rgba(0, 0, 0, 0.25);
}

h1, h2, h3, h4{
  font-family: 'Righteous', sans-serif;
}

span, p, li {
  font-family: 'Titillium Web', sans-serif;
}

@media (width < 60rem) {
  iframe {
    height: 400px;
    width: 400px;
  }
}
</style>
