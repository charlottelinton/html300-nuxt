<template lang="html">
  <div class="accordion" id="accordionExample">
    <div v-for="faq in faqs" class="card">
      <div class="card-header" id="headingOne">
        <h2 class="mb-0">
          <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
            {{ faq.title }}
          </button>
        </h2>
      </div>
      <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#accordionExample">
        <div class="card-body">
          {{ faq.text }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      faqs: [
        {title: 'Can I rent a screen?', text: 'Stuff about screen rental'},
        {title: 'Can I drink beer in the auditorium?', text: 'Yes!'},
        {title: 'Can I get married in the cinema?', text: 'Sure'}
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
