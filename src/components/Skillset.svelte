<script>
  export let title;
  export let perc;
</script>

<style>
  .item {
    display: block;
    align-items: center;
  }
  .level-bar {
    height: 12px;
    display: inline-block;
  }
  .item-title {
    display: inline-block;
  }
  .level-bar {
    position: relative;
    width: 100%;
    height: 12px;
    top: 1px;
  }
  .level-bar-inner {
    height: 12px;
  }

  @media (min-width: 768px) {
    .item-title {
      width: 30%;
    }
    .level-bar {
      width: 70%;
      float: right;
    }
  }
</style>

<div class="item">
  <h3 class="item-title">{title}</h3>
  <div class="level-bar bg-gray-300">
    <div
      class="level-bar-inner bg-orange-400"
      style="width: {perc}%;"
      data-level={perc} />
  </div>
</div>
