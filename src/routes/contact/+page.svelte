<script>
  import Nav from "../../lib/components/Nav.svelte";
  import Footer from "../../lib/components/Footer.svelte";
</script>
<Nav />

<!-- Form Section -->

<h1 class="p-2 text-5xl md:text-7xl text-center">Contact</h1>
<p class="px-2 text-center text-xl">Send us an E-Mail with any questions you may have. Make sure to include your vehicles year, make and model for the best response</p>
<div class=" container flex flex-col items-center justify-center h-screen">
<form class=" bg-white border border-black border-2" action="mailto:qasltd01@gmail.com" method="GET">
  <div>
    <input class="text-xl" type="text" placeholder="Subject" name="subject" required />
  </div>
  <div>
    <textarea class="text-xl" placeholder="Your message" name="body" required></textarea>
  </div>
  <div>
    <button class="text-xl my-5" type="submit">Send</button>
  </div>
  </form>
</div>
<Footer />
<style>
      h1{
  font-family: 'Righteous', sans-serif;
}
textarea, input, button, p{
  font-family: 'Titillium Web', sans-serif;
}
  button:hover {
    background-color: #273fff;
    color: white;
  }
  form {
    padding: 3rem;
  }
  .container {
    height: 75vh;
  }
  input, textarea {
    width: 20rem;
    margin-top: 2rem;
    padding: 5px;
    border-bottom: 2px solid black;
  }
  button {
    border: 2px solid black;
    padding: .5rem;
    border-radius: 5rem;
  }
</style>