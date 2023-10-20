<script>
  import Step from "./Step.svelte";

  let steps = [
    {name: 'AI Image Generator', icon: ' fa-solid fa-cart-shopping', href: "https://zencraft.pages.dev/?fbclid=IwAR2TK43DzgKWVZC8SOAbsvJcBODd158wg3bGfIGYorcZW9Sznp4Ycsy-MJM"},
    {name: 'Digital Image E-commerce store', icon: ' fa-solid fa-list-check', href: "https://next-ecomm-fe.pages.dev/"},
    {name: 'Jobs Marketplace', icon: ' fa-solid fa-diagram-project', href: "https://first-svelte-app.pages.dev/"}
  ]

  let benefits = [
    {name:'a passionate developer', description: 'I pivoted to be a software developer in August 2023 and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.'},
    {name:'a product design and backend fanatic', description: 'Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.'},
    {name:'an excellent communicator with great business acumen', description: 'Previously being in the world of finance and co-founding an NFT project raising RM1.2 million, I have developed my soft-skills to work well in a successful team and contribute to non-technical areas as well'},
  ]


</script>

<main class=" flex flex-col flex-1 p-4">
  <section id="introPage" class=" grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class=" flex flex-col justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class=" font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi, I'm <span class="poppins text-violet-400">Shaun</span> Shanil Menezes <br/>Full Stack
        <span class="poppins text-violet-400">Developer</span>
      </h2>
    <p class="text-base sm:text-lg md:text-xl">
      My <span class="poppins text-violet-400">favourite tech</span> includes Javascript, Sveltekit, TailwindCSS, DaisyUI, Node.js, Express.js, Docker, AWS, Prisma & PostgreSQL!

    </p>
    <!-- <a class=" blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" href='#' target="_blank">
      <div class='absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200' />
      <h4 class=" relative z-9">Get in touch &rarr;</h4>
    </a> -->
    <a href="mailto:shaunshanil95@gmail.com" class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer">
      <div class='absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200'></div>
      <h4 class="relative z-9">Get in touch &rarr;</h4>
    </a>
  </div>
  <div class=" relative shadow-2xl grid place-items-center flex flex-col">
    <img src="images/profile.jpg" alt="profile pic" class="object-cover z-[2] max-h-[70vh]" />

  </div>

  </section>

  <section id="projects" class=" py-20 lg:py-32 flex flex-col gap-24">
    <div class=" flex flex-col gap-2 text-center">
      <h6 class=" text-lg sm:text-xl md:text-2xl">A few of my creative endeavours</h6>
      <h3 class=" font-semibold text-3xl sm:text-4xl md:text-5xl">Curious to <span class="poppins text-violet-400">see</span> my work? </h3>
      
    </div>
    <div class="flex flex-row justify-between">
      <a href="#" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>View Demo</p>
      </a>
      <a href="#" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>View Demo</p>
      </a>
      <a href="#" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>View Demo</p>
      </a>

    </div>
    <div class=" grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>Zez AI is an AI Image Generator created with <strong class=" text-violet-400">Sveltekit, Node.js, OpenAI API, Express.js, PostgreSQL, Prisma & Stripe.</strong> Images are stored and uploaded using Multer and Stripe is used for all transaction handling. CRUD application which allows users to login using JWT tokens, generate any image using AI based on their prompt, edit any image they upload, create a variation of an uploaded image, view creations, and download creations. Users are given 5 free prompts, and after that they will have to pay $10 to get a total of 50 prompts.
        </p>

      </Step>
      <Step step={steps[1]}>
        <p>Zez E-commerse is an digital image e-commerce store created with <strong class=" text-violet-400">Sveltekit, Node.js, AWS, Express.js, PostgreSQL, Prisma & Stripe.</strong> Images are stored and uploaded using AWS S3 buckets and Stripe is used for all transaction handling. CRUD application which allows users to login together with JWT access and refresh tokens, upload an image for sale, view their images for sale, delete their images for sale, and finally purchase an image.
        </p>

      </Step>
      <Step step={steps[2]}>
        <p>Zez Jobs is a job marketplace created with <strong class=" text-violet-400">Sveltekit and Pocketbase.</strong> The backend was set up using Pocketbase. Users can view jobs and filter based on skills and location. After signing up and logging in, employers can post a job, view their jobs and edit their jobs.
        </p>

      </Step>


    </div>

  </section>
  <section id="about" class=" py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div class=" flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
      <h6 class=" text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class=" font-semibold text-3xl sm:text-4xl md:text-5xl">A bit <span class="poppins text-violet-400">about</span>me</h3>
    </div>
    <p class=" mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am . . .

    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
      <div class=" flex gap-6 sm:gap-8">
        <p class=" poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
          0{index + 1}
        </p>
        <div class=" flex flex-col gap-6 sm:gap-8">
          <h3 class=" text-2xl sm:text-3xl md:text-5xl">
            {benefit.name}
          </h3>
          <p>{benefit.description}</p>
        </div>

      </div>
      {/each}

    </div>
    <h5 class=" text-2xl sm:text-3xl font-semibold text-center poppins">The <span class="text-violet-400 poppins"> Complete</span> Package
    </h5>
    <div class=" flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
      <table class=" bg-white text-slate-700 rounded text-center">
        <thead class=" border-b border-solid border-slate-200">
          <tr class="">
            <th />
            <th class=" whitespace-nowrap p-2 px-4">Candiate #1

            </th>
            <th class=" whitespace-nowrap p-2 px-4">Candiate #2

            </th>
            <th class=" whitespace-nowrap p-2 px-4">Candiate #3

            </th>
            <th class=" whitespace-nowrap bg-violet-700 text-white p-4 px-8">Me

            </th>

          </tr>

        </thead>
        <tbody>
          <tr class="border-b border-solid border-slate-200">
            <td class=" border-r border-solid border-white whitespace-nowrap pl-4 pr-8 py-4 font-semibold text-sm">Dedication

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-green-500"></i>

            </td>

          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td class=" border-r border-solid border-white whitespace-nowrap pl-4 pr-8 py-4 font-semibold text-sm">Critical Thought

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-green-500"></i>

            </td>

          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td class=" border-r border-solid border-white whitespace-nowrap pl-4 pr-8 py-4 font-semibold text-sm">Interpersonal Skills

            </td>
            <td><i class=" fa-solid fa-check text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-green-500"></i>

            </td>

          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td class=" border-r border-solid border-white whitespace-nowrap pl-4 pr-8 py-4 font-semibold text-sm">Programming Ability

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-xmark text-slate-500"></i>

            </td>
            <td><i class=" fa-solid fa-check text-green-500"></i>

            </td>

          </tr>
        </tbody>
      </table>

    </div>
    <div class=" mx-auto -mt-12 italic sm:hidden opacity-50">
      <p>Scroll to see more &rarr;</p>

    </div>
    <p class=" mx-auto">So why not invest?</p>

  </section>

</main>
