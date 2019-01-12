---
title: Project in Panorama, Thessaloniki
main_block: 'main-top.html'
main_classes: 'main-inner main-projects bg-projects'
background-ratio: '0.6'
place: Panorama
type: Villa
thumbnail: img/projects/Villa in Panorama,Thessaloniki-vertical.jpg
mainStyle: "background-image:url('../img/slider/Villa in Panorama,Thessaloníki.jpeg');"
projectDetail:
 - fadein: fadeInLeft
   title: A private villa originally constructed by Fatouro in 1964, which we built respecting the historicity of the building
   description: ''
   offset: col-md-offset-4
   img: img/projects/panorama/panorama_0551.jpg
 - fadein: fadeInRight
   title: Amongst the significant changes we accomplished is the transformation of the interior design so as to accommodate present needs without altering the authentic design
   description: ''
   offset: ''
   img: img/projects/panorama/panorama_0552.jpg
 - fadein: fadeInLeft
   title: the alteration of the environmental configuration along with the prosthesis of a pool
   description: ''
   offset: col-md-offset-4
   img: img/projects/panorama/panorama_0554.jpg
   
---
<section class="project-details">
  <div class="container">
  {% for detail in page.projectDetail %}
    <div class="project-details-item">
      <div class="row">
        <div class="project-details-info wow {{ detail.fadein }}">
          <h3 class="project-details-title">{{ detail.title }} </h3>
          <p class="project-details-descr">{{ detail.description }}</p>
        </div>
        <div class="project-details-img col-md-8 {{ detail.offset }}">
          <img alt="" class="img-responsive" src="{{ detail.img | relative_url }}">
        </div>
      </div>
    </div>
  {% endfor %}
  </div>
</section>