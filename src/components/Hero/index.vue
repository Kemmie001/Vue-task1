<template>
  <article class="grid hero__article">
    <aside class="grid__col-1">
      <h1 class="grid__col-1--head">{{title}}</h1>
      <span class="span"> <span class="font-bold">at </span>
      <h1 class="grid__col-1--head span__head">{{company}}</h1>
      </span>
      <p v-if="companySummary" class="grid__col-1--para">{{companySummary}}</p>
      <button class="hero__button"><a class="hero__button--link" :href="companyUrl">VIEW COMPANY</a></button>
      <button class="hero__button"><a class="hero__button--link" href="">APPLY FOR THIS JOB</a></button>
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