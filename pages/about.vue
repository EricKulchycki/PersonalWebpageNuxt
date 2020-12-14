<template>
  <div>
    <div class="flex justify">
      <Header title="about me." />
    </div>
    <h3>
      personal.
    </h3>
    <p>
      i am a 24 year old canadian, living in manitoba, and working in the agriculture technology sector.
      in decemeber 2019 i graduated from the University of Manitoba with a BSc. in Computer Science, with a specialization in software developement.
      in my spare time i enjoy cooking, shitty 90's sitcoms, and playing disc golf! 
      A lot of what i do on weekends changes based on the season. separation of work and personal life is important, 
      so i have a lot of hobbies to keep me busy.
    </p>
    <h3>
      development.
    </h3>
    <div class="flex space-evenly">
      <div>
        <h5>languages.</h5>
        <div>
          <ul class="check-list">
            <li>javascript</li>
            <li>python</li>
            <li>java</li>
            <li>c</li>
          </ul>
        </div>
      </div>
    
      <div>
        <h5>frontend web frameworks.</h5>
        <div>
          <ul class="check-list">
            <li>react</li>
            <li>vue</li>
            <li>nuxt</li>
            <li>emberjs</li>
          </ul>
        </div>
      </div>
      <div>
        <h5>backend web frameworks.</h5>
        <div>
          <ul class="check-list">
            <li>laravel</li>
            <li>express</li>
            <li>spring</li>
            <li>chalice</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.check-list {
  margin: 0;
  padding: 0;
}

.check-list li {
  position: relative;
  list-style-type: none;
  padding-left: 2.5rem;
  margin-bottom: 0.5rem;
}

.check-list li:before {
    content: '';
    display: block;
    position: absolute;
    left: 0;
    top: -2px;
    width: 5px;
    height: 11px;
    border-width: 0 2px 2px 0;
    border-style: solid;
    border-color: #00a8a8;
    transform-origin: bottom left;
    transform: rotate(45deg);
}
</style>
