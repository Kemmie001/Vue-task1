<template>
    <div class="">
           <h3 class="paragraph">Skills</h3>
           <ul class="main__skills" >
             <li class="list--item main__skills__list" v-for="skill in skills" :key="skill">{{skill}}</li>
           </ul>
    </div>
</template>
<script>
export default {
    data(){
        return{
            skills:["BASIC ANIMATION", "PROJECT MANAGEMENT", "WIREFRAMES",
            "PROTOTYPES", "PHOTOSHOP", "USER INTERFACE", "USER EXPERIENCE" ]
        }
    }
}
</script>