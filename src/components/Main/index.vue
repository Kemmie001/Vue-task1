<template>
    <div class="main__about">
        <h1 class="gray para">About this role</h1>
          <div class="flex">
            <span class="black-box">
              CIRLCEBOX
            </span>
            <span class="">
              <h3 class="margin--left">{{title}} <span class="gray">{{type}}</span></h3>
              <p class="dark-gray margin--left">{{company}} - {{jobLocation}}</p>
              <h4 class=" margin--left">{{benefit}} </h4>
            </span>
          </div>
          <p class="paragraph">Lorem ipsum dolor, sit amet consectetur 
            adipisicing Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsam ipsa odio adipisci, fuga odit doloremque quasi, sapiente laborum commodi sed laudantium magnam maiores nemo 
            voluptatem eos ullam animi eum dicta! elit. 
            Ex earumrunt consectetur, quidem veniam laudantium.</p>
    </div>
</template>
<script>
export default {
  name: 'Role',
  props: {
    title: {
      type: String,
      required: true
    },
    type:{
        type: String,
        required:true,
    },
    company: {
      type: String,
      required: true
    },
    jobLocation:{
        type:String,
        required:true,
    },
    benefit:{
        type:String,
        required:true,
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