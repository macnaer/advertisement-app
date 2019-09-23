<script>
  import AdvItem from "./AdvItem.svelte";
  export let advs;
</script>

<style>
  section {
    width: 100%;
    display: grid;
    grid-template-columns: 1fr;
    grid-gap: 1rem;
  }

  @media (min-width: 768px) {
    section {
      grid-template-columns: repeat(2, 1fr);
    }
  }
</style>

<section id="meetups">
  {#each advs as adv}
    <AdvItem
      title={adv.title}
      subtitle={adv.subtitle}
      description={adv.description}
      imageUrl={adv.imageUrl}
      email={adv.contactEmail}
      address={adv.address} />
  {/each}
</section>
