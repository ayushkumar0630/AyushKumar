<template>
  <div class="main-wrapper">
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top" id="sideNav"> 
      <a class="navbar-brand js-scroll-trigger" href="#about">
        <span class="d-block d-lg-none">Start Bootstrap</span>
        <span class="d-none d-lg-block">
          <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="./assets/profile.jpg" alt="">
        </span>
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#education">Education</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#interests">Interests</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#awards">Awards</a>
          </li>
        </ul>
      </div>
    </nav>

    <div class="container-fluid p-0">

      <section class="resume-section p-3 p-lg-5 d-flex d-column" id="about">
        <div class="my-auto">
          <h1 class="mb-0">{{ name }}
            <span class="text-primary">{{ surname }}</span>
          </h1>
          <div class="subheading mb-5">{{ address }}
            <a href="mailto:name@email.com">{{ email }}</a>
          </div>
          <p class="mb-5">{{ aboutMe }}</p>
          <ul class="list-inline list-social-icons mb-0">
            <li class="list-inline-item">
            </li>
            <li class="list-inline-item">
              <a href="https://twitter.com/TheLegitAyush">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-twitter fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://www.linkedin.com/in/ayush-kumar-7629a240/">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-linkedin fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://github.com/ayushkumar0630">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
          </ul>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="experience">
        <div class="my-auto">
          <h2 class="mb-5">Experience</h2>

          <div class="resume-item d-flex flex-column flex-md-row mb-5" v-for="job in experience" :key="job.description">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">{{ job.position }}</h3>
              <div class="subheading mb-3">{{ job.company }}</div>
              <p>{{ job.description }}</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">{{ job.startDate }} - {{ job.endDate }}</span>
            </div>
          </div>

        </div>

      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="education">
        <div class="my-auto">
          <h2 class="mb-5">Education</h2>

          <div class="resume-item d-flex flex-column flex-md-row mb-5">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">University of Illinois Urbana-Champaign</h3>
              <div class="subheading mb-3">Bachelor of Science</div>
              <div>Computer Engineering - Concentration in Cryptography and Security</div>
              <p>GPA: 3.10</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">August 2014 - May 2018</span>
            </div>
          </div>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="skills">
        <div class="my-auto">
          <h2 class="mb-5">Skills</h2>

          <div class="subheading mb-3">Programming Languages &amp; Tools</div>
          <ul class="list-inline list-icons">
            <li class="list-inline-item">
              <i class="devicons devicons-html5"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-css3"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-javascript"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-bootstrap"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicon-vuejs-plain"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-python"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicon-linux-plain"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicon-oracle-original"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicon-amazonwebservices-original"></i>
            </li>
          </ul>

          <div class="subheading mb-3">Other Skills</div>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-check"></i>
              Scaling Businesses</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Machine Learning</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Leading Technical And Non-Technical Teams</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Agile Development &amp; Scrum</li>
          </ul>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="interests">
        <div class="my-auto">
          <h2 class="mb-5">Interests</h2>
          <p class="mb-2">When I am not working, I like to work on music. I am an amateur music producer and am always looking to learn more. My love from music comes from my fact that I have always been interested in music and still play the flute.</p>
          <p class="mb-2">I am also a practioner of meditation. I have been to to ashrams in India where I honed in my meditation skills and learned more about yoga. I continue to practice both things and both things play a large part in my life.</p>
          <p class="mb-2">Finally, I love to hike. Something about hiking makes be feel very relaxed and its an amazing feeling being so close to nature. I have completed some great hikes in the Himalayas and Appalachian mountains and am always looking foward to hiking new mountains.</p>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="awards">
        <div class="my-auto">
          <h2 class="mb-5">Awards &amp; Certifications</h2>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-trophy"></i>
              AWS Cloud Practioner</li>
            <li>
              <i class="fa-li fa fa-trophy"></i>
              1<sup>st</sup>
              Place - COZAD New Venture Competition 2018</li>
            <li>
              <i class="fa-li fa fa-trophy"></i>
              Paul Magelli Prize 2018</li>
            <li>
              <i class="fa-li fa fa-trophy"></i>
              2<sup>nd</sup>
              Place - Final Four Pitch Competition 2018</li>
            <li>
              <i class="fa-li fa fa-trophy"></i>
              HAX Accelerator - Cohort 12</li>
            <li>
            <li>
              <i class="fa-li fa fa-trophy"></i>
              iVenture Acclerator - Cohort 3</li>
          </ul>
        </div>
      </section>

    </div>
  <link rel="stylesheet" href="https://cdn.rawgit.com/konpa/devicon/df6431e323547add1b4cf45992913f15286456d3/devicon.min.css">
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'My portfolio',
      name: 'AYUSH',
      surname: 'KUMAR',
      address: '12347 BURNT PRAIRIE LANE · FRISCO, TX 75035 · (309) 533-8039 ·',
      email: 'ME@AYUSHKUMAR.XYZ',
      aboutMe: 'I am experienced in scaling startups and delivering successful outcomes for businesses. My businesses have been through the most competitive accelerators and raised money to impact those around the world. Currently, I am working on building Vitrix Health where we are building oral cancer screening tools that can scale globally and have impact on those in emerging economies. I am leveraging my past experience as a consultant and venture capital fellow to guide my decisions and grow this company into something that bring impact to the world.',
      experience: [
        {
          position: 'Chief Executive Officer',
          company: 'Vitrix Health',
          description: 'We are building an oral cancer screening device that allows for quicker and more accurate cancer screenings. Our solution is meant for global health, allowing it to scale well when selling to different countries around the world. Currently we are in HAX accelerator which is one of the most competitive acclerators in the world. Our device is currently undergoing testing and will be FDA compliant in the upcoming months.',
          startDate: 'March 2017',
          endDate: 'Present'
        },
        {
          position: 'Senior Fellow',
          company: 'IllinoisVENTURES',
          description: 'As the senior fellow I was responsible for maintaining a strong pipeline of companies that we could potentially invest in. After identifying different emerging startups, I would be responsible for writing investment memos that judged the startup\'s ability to succeed. Finally, I made sure every quarter to provide valuations of all our portfolio companies.',
          startDate: 'May 2017',
          endDate: 'May 2018'
        },
        {
          position: 'Cybersecurity Associate',
          company: 'PricewaterhouseCoopers Consulting',
          description: 'My role was to provide clients with insights on how to build a more robust security team and processes. During my time at PwC, I was working with C-level executives to build their security teams. I also provided insight on different market trends and how our clients could implement those offerings in their company.',
          startDate: 'August 2018',
          endDate: 'February 2019'
        },
        {
          position: 'Student Director',
          company: 'EntreCORPS Consulting',
          description: 'While leading the firm, my role was to directly source clients to work with. From there, I was responsible for creating SOWs and setting up projects for the length of a semester. I also worked with university leaders to use our firm as a way to grow the entrepreneurship ecosystem on campus.',
          startDate: 'August 2016',
          endDate: 'May 2018'
        }
      ]
    }
  },
  mounted () {
    const $ = this.jquery
    this.$nextTick(() => {
      // our custom jQuery code goes here
      $('a.js-scroll-trigger[href*="#"]:not([href="#"])').click(function () {
        if (location.pathname.replace(/^\//, '') === this.pathname.replace(/^\//, '') && location.hostname === this.hostname) {
          var target = $(this.hash)
          target = target.length ? target : $('[name=' + this.hash.slice(1) + ']')
          if (target.length) {
            $('html, body').animate({
              scrollTop: (target.offset().top)
            }, 1000, 'easeInOutExpo')
            return false
          }
        }
      })
      // Closes responsive menu when a scroll trigger link is clicked
      $('.js-scroll-trigger').click(function () {
        $('.navbar-collapse').collapse('hide')
      })
      // Activate scrollspy to add active class to navbar items on scroll
      $('body').scrollspy({
        target: '#sideNav'
      })
    })
  }
}
</script>

<style>
  body {
    font-family: 'Open Sans', serif;
    padding-top: 54px;
    color: #868e96;
  }
  @media (min-width: 992px) {
    body {
      padding-top: 0;
      padding-left: 17rem;
    }
  }
  h1,
  h2,
  h3,
  h4,
  h5,
  h6 {
    font-family: 'Saira Extra Condensed', serif;
    font-weight: 700;
    text-transform: uppercase;
    color: #343a40;
  }
  h1 {
    font-size: 6rem;
    line-height: 5.5rem;
  }
  h2 {
    font-size: 3.5rem;
  }
  .subheading {
    text-transform: uppercase;
    font-weight: 500;
    font-family: 'Saira Extra Condensed', serif;
    font-size: 1.35rem;
  }
  .list-social-icons a {
    color: #495057;
  }
  .list-social-icons a:hover {
    color: #017aff ;
  }
  .list-social-icons a .fa-lg {
    font-size: 1.75rem;
  }
  .list-icons {
    font-size: 3rem;
  }
  .list-icons .list-inline-item i:hover {
    color: #017aff ;
  }
  #sideNav .navbar-nav .nav-item .nav-link {
    font-weight: 600;
    text-transform: uppercase;
  }
  @media (min-width: 992px) {
    #sideNav {
      text-align: center;
      position: fixed;
      top: 0;
      left: 0;
      display: flex;
      flex-direction: column;
      width: 17rem;
      height: 100vh;
    }
    #sideNav .navbar-brand {
      display: flex;
      margin: auto auto 0;
      padding: 0.5rem;
    }
    #sideNav .navbar-brand .img-profile {
      max-width: 10rem;
      max-height: 10rem;
      border: 0.5rem solid rgba(255, 255, 255, 0.2);
    }
    #sideNav .navbar-collapse {
      display: flex;
      align-items: flex-start;
      flex-grow: 0;
      width: 100%;
      margin-bottom: auto;
    }
    #sideNav .navbar-collapse .navbar-nav {
      flex-direction: column;
      width: 100%;
    }
    #sideNav .navbar-collapse .navbar-nav .nav-item {
      display: block;
    }
    #sideNav .navbar-collapse .navbar-nav .nav-item .nav-link {
      display: block;
    }
  }
  section.resume-section {
    border-bottom: 1px solid #dee2e6;
    padding-top: 5rem !important;
    padding-bottom: 5rem !important;
  }
  section.resume-section .resume-item .resume-date {
    min-width: none;
  }
  @media (min-width: 768px) {
    section.resume-section {
      min-height: 100vh;
    }
    section.resume-section .resume-item .resume-date {
      min-width: 18rem;
    }
  }
  @media (min-width: 992px) {
    section.resume-section {
      padding-top: 3rem !important;
      padding-bottom: 3rem !important;
    }
  }
  .bg-primary {
    background-color: linear-gradient(to bottom, #33ccff 0%, #017aff 100%) !important;
  }
  .text-primary {
    color: linear-gradient(to bottom, #33ccff 0%, #017aff 100%)  !important;
  }
  a {
    color: linear-gradient(to bottom, #33ccff 0%, #017aff 100%) ;
  }
  a:hover, a:focus, a:active {
    color: linear-gradient(to bottom, #33ccff 0%, #017aff 100%) ;
  }
</style>
