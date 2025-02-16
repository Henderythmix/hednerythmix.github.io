<script setup>
import TitleCard from '@/components/TitleCard.vue'
import Project from '@/components/Project.vue';
import Hero from '@/components/Hero.vue';
import LinkPage from '@/components/LinkPage.vue';
</script>

<template>
  <main>
    <Hero>
      <div>
        <TitleCard />
        <h1>Computer Engineering Student</h1>
      </div>
      <div>Scroll for more</div>
      <div id="arrow-down"><a href="#about"><i class="bi bi-chevron-double-down"></i></a></div>
    </Hero>
    <p id="about">
      During my highscool years, I have learned to code by myself through online resources in fields such as Web development in HTML and CSS, small tools in Python, and game development in both Unity, and Love2D. Since then, I have studied at Simon Fraser University since 2022 in languages such as C++, Java, VHDL and Matlab which have not only taught me to program more optimally, but take my existing knowledge and skills to the next level. Not only have I worked with programming, but I have also learned to design hardware with VHDL.
    </p>

    <h1>Experience</h1>
    <p>All work experiences within tech, whether they are actual jobs or volunteer experiences</p>
    <div class="grid">
      <Project title="ESSS Website" date="June 2023-Present" link="https://esss.ca">
        Designed a maintainable website for the Engineering Student Society at Simon Fraser University. Maintained it since approximately June 2023.
      </Project>
      <Project title="SFU Robot Soccer" date="January-April 2024" link="https://www.sfurobotsoccer.com/">
        Although there was no redesigning for this club, I was responsible for maintaining the website for the SFU Robot Soccer team from January 2024 to April 2024
      </Project>
    </div>

    <h1>Team Projects</h1>
    <div class="grid">
      <Project title="Duogotchi" date="October 2024" link="https://github.com/Henderythmix/duogotchi">
        For a 24-hour hackathon in October 2024, I lead and designed a tamagotchi inspired web app prototype for couples to virtually take care of each other.
      </Project>
      <Project title="VHDL Calculator" date="December 2023" link="https://github.com/Henderythmix/FPGA-Calculator">
        Developed a calculator in VHDL to be used on a Cyclone IV E FPGA board with a team of two other students in a class for a project.
      </Project>
      <Project title="Automated Toilet Paper Reloader" date="September-December 2022" link="https://github.com/Henderythmix/ToiletPaperware">
        In a team of seven, we designed and implemented an automated toilet paper reloader for a class project to present to the school. Although the hardware design does not exist any more, the software code still exists for the project.
      </Project>
      <Project title="P.A.W.N.S" date="February 2021" link="https://dylanstil.itch.io/pawns-the-survival-game-of-staying-together">
        Team of four where we made a game in Unity for Brackeys Game Jam 2021.1. This was a difficult project as there was a snow storm in texas so half our team lost signal, but we managed to make a prototype worth sharing. This was a project done before my engineering degree started.
      </Project>
    </div>

    <h1>Personal Projects</h1>
    <div class="grid">
      <Project title="Mariana's Trench" date="August 2023" link="https://github.com/Henderythmix/MarianasTrench">
        Designed for Brackeys Jam 2023.2, This game was made in C++ and raylib after going through a whole year of studying C++.
      </Project>
      <Project title="Triple-M" date="April 2023-December 2023" link="https://github.com/Henderythmix/Triple-M">
        For the experience, I created a markup language compiler that takes its its own language, tokenizes it, and converts the data into an html file. I eventually tested this on the ESSS website to easily develop the website without being overwhelmed by angle brackets
      </Project>
    </div>
    <Project title="Snakelock" date="August 2022" link="https://github.com/Henderythmix/SnakeLock">
      By learning C++ before starting to study engineering, I put my knowledge to the test by making a snake inspired game in C++ using raylib for Untitled Game Jam.
    </Project>

    <h1>Other Projects</h1>
    <p>Above are all my achievements that I think are either most relevant to my experience, or the most presentable on a resume. If you want to see my other projects, you can find them on my github below:</p> 
    <LinkPage title="Github" link="https://github.com/Henderythmix" icon="bi-github" />
  
  </main>
</template>

<style lang="scss" scoped>
p {
  text-indent: 4rem;
  max-width: 50%; 
}

.grid {
  justify-items: center;
}

.box-container {
  width: 390px;
  height: calc(100% - 2rem);
}

@media only screen and (max-width: 450px) {
  p {
    max-width: 90%;
  }

  .box-container {
    width: 85%;
  }
}

#arrow-down {
  margin-top: 2rem;

  &:hover {
    transform: translate(0, 5px);
  }
}

#about {
  padding-top: 3rem;
}
</style>
