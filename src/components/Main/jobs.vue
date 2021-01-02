<template>
    <div>
        <h3 class="paragraph">{{title.first}}<span class="gray">{{type}}</span></h3>
          <p class="job--m-bottom">{{company}} - {{jobLocation}}</p>
          <h3 class="paragraph">{{title.second}} <span class="gray">{{type}}</span></h3>
          <p class="jobs--m-bottom">{{company}} - {{jobLocation}}</p>
          <h3 class="paragraph"> {{title.third}} <span class="gray">{{type}}</span></h3>
          <p class="jobs--m-bottom">{{company}} - {{jobLocation}}</p>
        <buton class="green-btn">
          <a href="" class="green-btn__link">Apply for the job</a>
        </buton>
    </div>
</template>
<script>
export default {
    name: "Jobs",
    props:{
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
    },
    data(){
        return{
           title:{
            first: "Senior UI/UX Designer",
            second: "Web Developer",
            third: "Junior Designer"
           },
        }
    }
}
</script>