<template>
  <div class="container">
    <header class="header">
      <Navbar class="header__navbar"></Navbar>
      <Hero class="header__hero" title="Senior UX/UI Designer" company="Circlebox Creative" companySummary="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex earumrunt consectetur, quidem veniam laudantium."></Hero>
    </header>
    <section class="">
       <article class="grid my-2">
        <aside class="col-1">
          <Role 
          title="Senior UX/U1 Designer" 
          type="(Full Time)" 
          company="Circlebox Creative" 
          jobLocation="Royston, Herrtfordshire, UK"
          benefit="&euro;35-45,000 + Benefits"
          />
           <Skill/>
           <Description/>
        </aside>
        <aside class="col-2">
          <button class="green-btn">
            <a href="" class="green-btn__link">Apply for the job</a>
          </button>
          <button class="btn">
            <a class="link" href=""><i class="fab fa-facebook"></i>
            Share on Facebook
            </a>
          </button>
          <button class="btn">
            <a class="link" href=""><i class="fab fa-twitter"></i>
            Share on Twitter
            </a>
          </button>
          <button class="btn">
            <a class="link" href=""><i class="fab fa-linkedin-in"></i>
            Share on LinkedIn
            </a>
          </button>
          <joblink/>
          <p class="para"><span class="gray">More from </span><a href="" class="blue">Circlebox
             Creative</a></p>
          <jobs
          type="(Full Time)" 
          company="Circlebox Creative" 
          jobLocation="Royston, Herrtfordshire, UK"/>
        <p class="paragraph"><span class="gray">Looking for employees </span><a href="" class="blue">Post a job!</a></p>
        </aside>
       
      </article>
    </section>
  </div>
  
</template>

<script>
import Navbar from '../components/Navbar'
import Hero from '../components/Hero'
import Role from '../components/Main/index'
import Skill from '../components/Main/skills'
import Description from '../components/Main/description'
import Joblink from '../components/Main/joblink'
import Jobs from '../components/Main/jobs'
export default {
  name: 'Base',
  props: {
    msg: String
  },
  components: {
    Navbar, Hero,
    Role, Skill,
    Description, Joblink,
    Jobs
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
*{
  padding: 0;
  margin: 0;
}
#app {
  font-family: Arial, sans-serif;
  
}
  .header{
    color: #ffff;
    background-color: rgb(35, 170, 223);
  }
  .navbar--brand-name{
    font-size: 1rem;
    font-weight: bold;
  }
  .flex{
    display: flex;
    list-style: none;
  }
  .list--item{
    margin: 0.5rem;
  }
  .left{
    margin-left: auto;
    margin-top: 0.5rem
  }
  .left__list{
    font-size: 0.7rem
  }
  .list--item__link{
    color: #fff;
    text-decoration: none;
  }
  .user{
    display: inline-block;
    background-size: cover;
    border-radius: 50%;
    width: 30px;
    height:30px;
    background-image: url('../assets/human.jpg');
  }
  .grid{
    display: grid;
    grid-gap: 2rem;
    margin-top: 2rem;
    grid-template-columns: 50% 30%;
    justify-content: center;
    align-content: center;
  }
  
  .hero__article{
    margin-top:3rem;
    padding-bottom: 1rem;
  }
  .grid__col-1--head{
    font-size: 1.9rem;
    line-height: 30px;
    width: 100%;
  }
  .grid__col-1--para{
    font-size: 0.8rem;
    line-height: 15px;
    word-spacing: 0.2rem;
    font-weight: 300;
    color: hsla(0, 0%, 100%, 0.7);
    padding-bottom: 0.5rem;
    width: 80%;
    
  }
  .span__head{
    display: inline;
    word-spacing: 0.3rem;
  }
  .span{
    display: block;
    padding-bottom: 1rem;
    
  }
  .font-bold{
    color: hsla(0, 0%, 100%, 0.9);
    font-size: 1.5rem;
    font-weight: 50;
  }
  .hero__button{
    border: none;
    background-color: rgba(43, 109, 134, 0.5);
    border-radius: 0.3rem;
    margin-top: 1rem;
    margin-right: 1rem;
    padding: 1rem;
  }
  .hero__button--link{
    text-decoration: none;
    color:#ffffff;
    font-weight: bold;
  }
  .gray{
    color: hsla(340, 1%, 46%, 0.7);
    padding-bottom: 1rem;
  }
  .margin--left{
    margin-left: 1rem;
    margin-top: 0.5rem;
  }
  .black-box{
    background-color: black;
    color: #fff;
    font-size: 0.7rem;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 0.3rem;
    height: 100px;
    width: 100px;
    font-weight: bold;
  }
  .paragraph{
    line-height: 25px;
    padding-top: 1rem;
    padding-bottom: 0.5rem;
  }
  .main__skills{
    list-style: none;
    margin-bottom: 1rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr) );
  }
  .main__skills__list {
    border: rgb(35, 170, 223) solid 2px;
    text-align: center;
    font-size: 0.7rem;
    font-weight: bold;
    border-radius: 0.3rem;
    padding: 0.5rem;
  }
  .jobs--m-bottom{
    margin-bottom: 1rem;
  }
  .green-btn{
    display: block;
    padding: 0.5rem;
    background: #509c85;
    margin-top: 0.5rem;
    width: 90%;
    /* box-shadow:hsla(0, 4%, 91%, 0.7) 1px 1px 1px 1px; */
    border: none;
    border-radius: 0.3rem;
    text-align: center;
    font-weight: bold;
  }
  .green-btn__link{
    
    color: #fff;
    text-decoration: none;
  }
  .blue-btn{
    position: absolute;
    top: 0;
    right: 0;
    height: 100%;
    border-bottom-right-radius: 0.2rem;
    border-top-right-radius: 0.3rem;
    background-color: rgb(35, 170, 223);
    color: white;
    padding-right: 0.7rem;
    padding-left: 0.5rem;
    display: flex;
    align-items: center;
    /* padding-bottom: 0.5rem; */
    
  }
  .btn{
    position: relative;
    display: block;
    padding: 0.5rem;
    background: transparent;
    margin-top: 1rem;
    width: 90%;
    box-shadow:hsla(0, 4%, 73%, 0.7) 1px 1px 1px 1px;
    border: none;
    border-radius: 0.3rem;
  }
  .fab{
    margin-right: 1rem;
    /* color: rgb(35, 170, 223); */
  }
  .fa-twitter{
    color: rgb(35, 170, 223);
  }
  .fa-facebook{
    color:rgb(37, 37, 209);
  }
  .fa-linkedin-in{
    color: rgb(9, 39, 95);
  }
  .link{
    text-decoration: none;
    color: black;
  }
  .job{
    margin-top: 2rem;
    margin-bottom: 2rem;
  }
  .job__paragraph{
    color: hsla(340, 1%, 46%, 0.7);
  }
  .gray-link{
    float: left;
    color: hsla(340, 1%, 46%, 0.7);
    text-decoration: none;
    font-size: 1rem
  }
  .blue{
    text-decoration: none;
    color: rgb(35, 170, 223);
    font-weight: bold;
  }
  @media screen and (max-width:1024px){
    .grid{
      margin-top: 1.5rem;
      grid-template-columns: 90%;
    }
  }
  @media screen and (min-width:1100px) {
    .left__list{
      font-size: 1rem;
      padding-top: 0.5rem;
    }
    .navbar--brand-name{
      font-size: 1.5rem;
      padding: 0.5rem;
    }
    .hero__article{
      line-height: 45px;
      font-size: 2.7rem;
    }
    .font-bold{
      font-size: 2.2rem;
  }
    .grid__col-1--para{
      width: 80%;
      font-size: 1.3rem;
      line-height: 30px;
    }
  }
</style>


