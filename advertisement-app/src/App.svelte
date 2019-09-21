<script>
  import Header from "./UI/Header.svelte";
  import AdvItem from "./Adv/AdvItem.svelte";

  const advs = [
    {
      id: "a1",
      title: "Front end trends",
      subtitle: "Super events1",
      description: "Good speaker!2",
      imageUrl:
        "https://www.swarmonline.com/wp-content/uploads/2017/09/evolution-of-javascript.png",
      address: "Soborna street",
      contactEmail: "support@itstep.org"
    },
    {
      id: "a2",
      title: "Victim of Agile",
      subtitle: "Super events2",
      description: "Good speaker!1",
      imageUrl:
        "https://www.sam-solutions.com/blog/wp-content/uploads/2018/07/AGILE@2x-704x371.png",
      address: "Soborna street",
      contactEmail: "support@itstep.org"
    }
  ];
</script>

<style>
  main {
    margin-top: 5rem;
  }
</style>

<Header />
<main>
  {#each advs as adv}
    <AdvItem
      title={adv.title}
      subtitle={adv.subtitle}
      description={adv.description}
      imageUrl={adv.imageUrl}
      email={adv.contactEmail}
      address={adv.address} />
  {/each}

</main>
