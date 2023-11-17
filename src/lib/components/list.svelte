<script>
  let myList = [
    {
      name:"Bob",
      id:'1'
    },
    {
      name:"Charles",
      id:'2'
    },
    {
      name:"James",
      id:'3'
    }
  ]
</script>

<h3 class="h3">List of People</h3>
<ul class="m-auto max-w-xl">
  {#each myList as person}
		<li class="border-token">{person.name} has id of {person.id}</li>
	{/each}
</ul>