<template>
<div>
  <searchBar/>
  <popDirections/>
</div>
</template>

<script>
import searchBar from '../components/search-bar.vue';
import popDirections from '../components/pop-directions.vue';
export default {
  name: 'IndexPage',

  components: {
    searchBar, popDirections
  }
}
</script>
