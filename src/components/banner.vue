<template>
  <div class="container">
    <header>
      <Navbar></Navbar>
      <Hero title="Senior UX/UI Designer" company="Circlebox Creative" companySummary="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex earumrunt consectetur, quidem veniam laudantium."></Hero>
    </header>

    <section class="">
       <article class="grid my-2">
        <aside class="col-1">
          <h1 class="gray para">About this role</h1>
          <div class="flex">
            <span class="black-box">
              CIRLCEBOX
            </span>
            <span class="">
              <h3 class="ml">Senior UX/U1 Designer <span class="gray">(Full Time)</span></h3>
              <p class="dark-gray ml">Circlebox Creative - Royston, Herrtfordshire, UK</p>
              <h4 class=" ml">&euro;35-45,000 + Benefits </h4>
            </span>
          </div>
          <p class="para">Lorem ipsum dolor, sit amet consectetur 
            adipisicing Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsam ipsa odio adipisci, fuga odit doloremque quasi, sapiente laborum commodi sed laudantium magnam maiores nemo 
            voluptatem eos ullam animi eum dicta! elit. 
            Ex earumrunt consectetur, quidem veniam laudantium.</p>
         <div class="">
           <h3 class="para">Skills</h3>
           <ul class="flex-skills">
             <li>USER EXPERIENCE</li>
             <li>USER INTERFACE</li>
             <li>PHOTOSHOP</li>
             <li>PROTOTYPES</li>
             <li>WIREFRAMES</li>
             <li>PROJECT MANAGEMENT</li>
             <li>BASIC ANIMATION</li>
           </ul>
           <h2>Description</h2>
          <p class="para">Are you creative, innovative and ahead of the industry standards? We want you on our leading-edge team!</p>
          <p class="para">
            As our UX/UI Designer, Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus laudantium similique ducimus aut esse, maxime tenetur dolorem ipsa? Odit praesentium dolore, recusandae laborum ipsum modi non quas eligendi voluptates voluptatem.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum veritatis sint dolor enim, commodi alias fugit optio iste repudiandae assumenda nihil esse impedit facere eaque delectus perspiciatis illo odit? Sit.
            You will create visuals/sketches work and be able to work and communicate with the development team to represent ides and new features that we want built and/or implemented.</p>
          <p class="para">You'll be running the UI/UX show which will include brsinstorming design and usability options, building simple wireframes and conducting usability tests.</p>
          <p class="para">The skillset:</p>
         <ul class="">
           <li>3+ years of industry/agency experience in a digital capacity</li>
           <li>Strong design portfolio that reflects a deep understanding of interaction design</li>
           <li>An understanding of design patterns and how design decisions have an impact on the implentation</li>
           <li>Well-developed communication skills including information ability to articulate creative concepts</li>
           <li>Solid understanding of web development processes including information architecture,  usability/user experience testing & quality assurance</li>   
           <li>Clear understanding of usability, user-centered design, and web standards</li>
         </ul>
         <p class="para">
           The who, what, where of us:
         </p>
         <p class="para">
           We started in a small, 2-bedroom apartment in Royston and have grown into a respectable digital design agency with clients all over the world. Over the years Circlebox Creative has gained a reputation of steady growth.
         </p>
         </div>
        </aside>
        <aside class="col-2">
          <button class="green-btn">
            <a href="">Apply for the job</a>
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
          <div class="job">
            <p class="">Job URL</p>
          <button class="btn">
            <a class="gray-link" href="">https://digitalprofile.io/circlebox/create
            </a><span class="blue-btn">Copy Link</span>
          </button>
          </div>
          <p class="para"><span class="gray">More from </span><a href="" class="blue">Circlebox
             Creative</a></p>
          <h3 class="para">Senior UX/U1 Designer <span class="gray">(Full Time)</span></h3>
          <p class="mt">Circlebox Creative - Royston, Hertfordshine, UK</p>
          <h3 class="para">Web Developer <span class="gray">(Full Time)</span></h3>
          <p class="mt">Circlebox Creative - Royston, Hertfordshine, UK</p>
          <h3 class="para"> Junior Designer <span class="gray">(Full Time)</span></h3>
          <p class="mt">Circlebox Creative - Royston, Hertfordshine, UK</p>
           <buton class="green-btn">
          <a href="" class="">Apply for the job</a>
        </buton>
        <p class="para"><span class="gray">Looking for employees </span><a href="" class="blue">Post a job!</a></p>
        </aside>
       
      </article>
    </section>
  </div>
  
</template>

<script>
import Navbar from '../components/Navbar'
import Hero from '../components/Hero'
export default {
  name: 'Base',
  props: {
    msg: String
  },
  components: {
    Navbar, Hero
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  header{
    color: #ffff;
    background-color: rgb(35, 170, 223);
  }
  .brand-name{
    font-size: 1rem;
    font-weight: bold;
  }
  .flex{
    display: flex;
    list-style: none;
  }
  li{
    margin: 0.5rem;
  }
  .left{
    margin-left: auto;
    margin-top: 0.5rem
  }
  .left li{
    font-size: 0.7rem
  }
  li a{
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
  
  .my{
    margin-top:3rem;
    padding-bottom: 1rem;
  }
  .my h1{
    font-size: 1.9rem;
    line-height: 30px;
    width: 100%;
  }
  .my p{
    font-size: 0.7rem;
    line-height: 15px;
    word-spacing: 0.2rem;
    font-weight: 300;
    color: hsla(0, 0%, 100%, 0.7);
    padding-bottom: 0.5rem;
    width: 80%;
    
  }
  .span h1{
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
  .my button{
    border: none;
    background-color: rgba(43, 109, 134, 0.5);
    
    border-radius: 0.3rem;
    margin-top: 1rem;
    margin-right: 1rem;
    padding: 1rem;
  }
  .my button a{
    text-decoration: none;
    color:#ffffff;
    font-weight: bold;
  }
  .gray{
    color: hsla(340, 1%, 46%, 0.7);
    padding-bottom: 1rem;
  }
  .ml{
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
  .para{
    line-height: 25px;
    padding-top: 1rem;
    padding-bottom: 0.5rem;
  }
  .flex-skills{
    list-style: none;
    margin-bottom: 1rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr) );
  }
  .flex-skills li {
    border: rgb(35, 170, 223) solid 2px;
    text-align: center;
    font-size: 0.7rem;
    font-weight: bold;
    border-radius: 0.3rem;
    padding: 0.5rem;
  }
  .mt{
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
  .green-btn a{
    
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
  .job p{
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
    .left li{
      font-size: 1rem;
      padding-top: 0.5rem;
    }
    .brand-name{
      font-size: 1.5rem;
      padding: 0.5rem;
    }
    .my h1{
      line-height: 45px;
      font-size: 2.7rem;
    }
    .font-bold{
      font-size: 2.2rem;
  }
    .my p{
      width: 70%;
      font-size: 1.3rem;
      line-height: 30px;
    }
  }
</style>
