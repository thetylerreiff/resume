<script>
  import Experience from "./components/Experience.svelte";
  import Skillset from "./components/Skillset.svelte";
</script>

<style>
  :global(body) {
    background-color: #dae2ec;
    padding: 1.5rem;
  }
  div {
    display: block;
  }

  .wrapper {
    max-width: 960px;
    margin: 0 auto;
    position: relative;
  }

  .sidebar-wrapper {
    position: static;
  }

  .body-wrapper {
    padding: 60px;
  }

  footer {
    display: flex;
    height: 100px;
    text-align: center;
    justify-content: center;
    align-items: center;
  }

  @media (min-width: 768px) {
    .sidebar-wrapper {
      width: 240px;
      position: absolute;
      min-height: 100%;
      right: 0;
    }

    .body-wrapper {
      padding: 60px;
      padding-right: 300px;
    }
  }
</style>

<main class="wrapper bg-white shadow-xl">
  <div class="sidebar-wrapper bg-orange-500 text-white">
    <div class="p-8 bg-orange-800 text-center">
      <img
        src="me.jpg"
        class="rounded-full h-32 w-32 mx-auto"
        alt="tyler reiff avater" />
      <h1 class="text-lg text-2xl font-bold text-white">Tyler J. Reiff</h1>
      <div>Software Engineer</div>
    </div>
    <div class="px-8 py-4">
      <div>
        <a href="mailto://reiff.tyler.j@gmail.com">reiff.tyler.j@gmail.com</a>
      </div>
      <div>
        <a href="https://reifflabs.com">reifflabs.com</a>
      </div>
      <div>
        <a href="https://linkedin.com/in/tyler-reiff">
          linkedin.com/in/tyler-reiff
        </a>
      </div>
      <div>
        <a href="https://github.com/reiff12">github.com/reiff12</a>
      </div>
      <div>
        <a href="https://twitter.com/tjrcodes">@tjrcodes</a>
      </div>
    </div>

    <div class="px-8 py-4">
      <h3 class="text-xl font-hairline">Education</h3>
      <div class="font-bold">University of Connecticut</div>
      <div class="text-md">
        Completed 70 credits toward a duel degree in chemisty & chemical
        engineering
      </div>
    </div>

    <div class="px-8 py-4">
      <h3 class="text-xl font-hairline">Languages</h3>
      <div class="text-md">
        English
        <span class="text-gray-100">(Native)</span>
      </div>
    </div>

    <div class="px-8 py-4">
      <h3 class="text-xl font-hairline">Interests</h3>
      <div class="text-md">Cooking</div>
      <div class="text-md">Photography</div>
    </div>

  </div>
  <div class="body-wrapper">

    <section class="py-4">
      <h2 class="text-xl font-bold">Career Path</h2>
      <p>
        I help small companies unlock the potential of their data. From web
        application to data platforms.
      </p>
    </section>

    <section class="py-4">
      <h2 class="text-xl font-bold">Experience</h2>
      <Experience
        company="IMCORP"
        title="Software Engineer, Signal Processing and Artificial Intelligence"
        date="July 2017"
        location="Manchester, CT">
        Develop scientific analysis tooling for web-based analysis of signal
        waveform data. Application stack includes React, WebAssembly, Node and
        Python. Assisted in architecting an automated data analysis system,
        built as a polyglot set microservices. Deployed as a containerized
        application on AWS. Founding member of the company's data science
        program. Implementing quality-assurance and accessibility measures in
        the data lake. Formalized a systematic approach to research.
      </Experience>

      <Experience
        company="Reifflabs"
        title="Founder & Developer"
        date="October 2015"
        location="San Francisco, CA">
        Develop custom enterprise and consumer web applications. Create HTML,
        CSS, JavaScript and wireframes to spearhead user-centered design efforts
        for dozens of web pages. Apply agile development methodology to project
        management. Managed IT infrastructure including Web Servers, DNS, object
        storage, and database administration.
      </Experience>

      <Experience
        company="Connecticut Business Systems"
        title="IT Support Specialist"
        date="July 2016 - February 2017"
        location="Wethersfield, CT">
        First point of contact for all IT issues. Ensured timely resolution of
        problems, reducing response time from 24 hours to minutes. Create custom
        software applications to solve business problems including tracking
        field technician ETA's. Compose documentation for non-technical end
        users.
      </Experience>
    </section>

    <section class="py-4">
      <h2 class="text-xl font-bold">Skills</h2>
      <Skillset title="JavaScript" perc={98} />
      <Skillset title="Python" perc={90} />
      <Skillset title="Data Viz" perc={85} />
      <Skillset title="System Design" prec={80} />
    </section>

  </div>
</main>

<footer>Made with ❤️ by Tyler J. Reiff</footer>
