<template>
  <article class="grid my">
    <aside class="col-1">
      <h1>{{title}}</h1>
      <span class="span"> <span class="font-bold">at </span>
      <h1>{{company}}</h1>
      </span>
      <p v-if="companySummary">{{companySummary}}</p>
      <button><a :href="companyUrl">VIEW COMPANY</a></button>
      <button><a href="">APPLY FOR THIS JOB</a></button>
    </aside>
    <aside class="col-2"></aside>
  </article>
</template>

<script>
export default {
  name: 'Banner',
  props: {
    title: {
      type: String,
      required: true
    },
    company: {
      type: String,
      required: true
    },
    companySummary: {
      type: String
    }
  },
  computed: {
    companyUrl(){
      return `https://company.co/${this.company}`
    }
  }
}
</script>

<style>

</style>