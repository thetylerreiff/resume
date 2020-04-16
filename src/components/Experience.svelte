<script>
  export let company;
  export let title;
  export let date;
  export let location;
</script>

<style>
  section {
    padding: 0.75rem;
    padding-right: 0;
    padding-left: 0;
  }
</style>

<section>
  <div>
    <span class="font-bold">{company}</span>
    {title}
  </div>
  <div class="font-hairline flex justify-between">
    <span>{location}</span>
    <span>{date}</span>
  </div>
  <p>
    <slot />
  </p>
</section>
