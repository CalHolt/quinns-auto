<script>
  import Nav from "../../lib/components/Nav.svelte";
  import Footer from "../../lib/components/Footer.svelte";

  let inspectionName = [
    "Pre-Purchase Inspection",
    "Out Of Province Inspection",
    "Insurance Inspection",
    "AMVIC Insepction",
    "48 Inspection",
    "Brake Inspection"
  ];
  let inspectionCost = [
    "$125.00",
    "$155.45",
    "$79.95",
    "$89.95",
    "$59.95",
    "$54.95"
  ];
  let routineService = [
    "Regular Oil Change",
    "Synthetic Oil Change",
    "Premium Oil Change",
    "Diesel Oil Change",
    "Mount and Balance",
    "P/S Flush",
    "Brake Flush",
    "Coolant Flush"
  ];
  let routinePrice = [
    "Starting at $82.43",
    "Starting at $100.00",
    "Starting at $175.00",
    "Starting at $220.00",
    "$33.75 per tire ",
    "$79.95",
    "$95.87",
    "Starting at $169.95"
  ];
  let repairName = [
    "Tire Repair",
    "Electrical Diagnostic",
    "Scan and Diagnose",
    "A/C Service 134A",
    "A/C Service 1234YF",
    "Charging System Test"
  ]
  let repairCost = [
    "$35.00 per tire",
    "$150.00/hour",
    "$165.00/hour",
    "$195.00",
    "$395.00",
    "$49.95"
  ]
</script>
<Nav />

<!-- Title Section -->

<h1 class="p-2 text-5xl md:text-7xl text-center">Services</h1>
<div class="px-2 text-center">
  <span>**All services provided by Quinn's Auto Service are subject to tax and shop fees**</span>
</div>

<!-- Price Section -->

<div class="my-2 py-4 prices flex flex-col">
  <h2 class="text-center text-3xl md:text-4xl p-4">Inspections</h2>
  <div class="list flex justify-center md:gap-12">
    <div class="flex flex-col align-right">
      {#each inspectionName as name}
      <span class="text-xl">{name}</span>
      {/each}
    </div>
    <div class="flex flex-col align-center">
      {#each inspectionCost as cost}
      <span class="text-xl">{cost}</span>
      {/each}
    </div>
  </div>
  <h2 class="text-center text-3xl md:text-4xl p-4">Routine Service</h2>
  <div class="list flex justify-center md:gap-12">
    <div class="flex flex-col align-center">
      {#each routineService as service}
      <span class="text-xl">{service}</span>
      {/each}
    </div>
    <div class="flex flex-col align-center">
      {#each routinePrice as price}
      <span class="text-xl">{price}</span>
      {/each}
    </div>
  </div>
  <h2 class="text-center text-3xl md:text-4xl p-4">Repairs</h2>
  <div class="list flex justify-center  md:gap-12">
  <div class="flex flex-col align-center">
    {#each repairName as repair}
    <span class="text-xl">{repair}</span>
    {/each}
  </div>
  <div class="flex flex-col align-center">
    {#each repairCost as cost}
    <span class="text-xl">{cost}</span>
    {/each}
  </div>
</div>
</div>
<Footer />
<style>
    h1, h2{
  font-family: 'Righteous', sans-serif;
}
span{
  font-family: 'Titillium Web', sans-serif;
}
@media (width > 50rem) {
  .prices {
    width: 40ch;
    margin: auto;
  }
  .list{
    justify-content: space-between;
  }
}


</style>