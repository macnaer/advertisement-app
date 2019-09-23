<script>
  import Header from "./UI/Header.svelte";
  import AdvList from "./Adv/AdvList.svelte";

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

  form {
    width: 30rem;
    max-width: 90%;
    margin: auto;
  }
</style>

<Header />
<main>
  <!-- <form on:submit|preventDefault={addMeetup}>
    <TextInput
      id="title"
      label="Title"
      type="text"
      value={title}
      on:input={event => (title = event.target.value)} />
    <TextInput
      id="subtitle"
      label="Subtitle"
      type="text"
      value={subtitle}
      on:input={event => (subtitle = event.target.value)} />
    <TextInput
      id="address"
      label="Address"
      type="text"
      value={address}
      on:input={event => (address = event.target.value)} />
    <TextInput
      id="imageUrl"
      label="Image URL"
      type="text"
      value={imageUrl}
      on:input={event => (imageUrl = event.target.value)} />
    <TextInput
      id="email"
      label="E-Mail"
      type="email"
      value={email}
      on:input={event => (email = event.target.value)} />
    <TextInput
      id="description"
      label="Description"
      controlType="textarea"
      value={description}
      on:input={event => (description = event.target.value)} />
    <Button type="submit" caption="Save" />
  </form> -->
  <AdvList {advs} />
</main>
