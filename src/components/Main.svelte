<script>
  import Step from "./Step.svelte";

  let steps = [
    {name: 'AI Image Generator', icon: ' fa-solid fa-cart-shopping', href: "https://zencraft.pages.dev/?fbclid=IwAR2TK43DzgKWVZC8SOAbsvJcBODd158wg3bGfIGYorcZW9Sznp4Ycsy-MJM", fe:"https://github.com/ssm53/zencraft", be:"https://github.com/ssm53/zencraftBE"},
    {name: 'Digital Image E-commerce store', icon: ' fa-solid fa-list-check', href: "https://next-ecomm-fe.pages.dev/", fe:"https://github.com/ssm53/Next-Ecomm-FE", be:"https://github.com/ssm53/Next-ecom-BE"},
    {name: 'Jobs Marketplace', icon: ' fa-solid fa-diagram-project', href: "https://first-svelte-app.pages.dev/", fe:"https://github.com/ssm53/first-svelte-app", be:"https://github.com/ssm53/first-svelte-app"}
  ]

  let benefits = [
    {name:'100% money back guaranteed', description: 'You heard that right, we only get paid if you are happy. Win-win.'},
    {name:'we will host your website forever', description: "You don't need to worry if your website will not function, forever"},
    {name:'free access to our AI chatbots', description: 'AI is cool. We are developing chatbots which can analyse any document. Imagine a ChatGPT but for your own documents'},
  ]


</script>

<main class=" flex flex-col flex-1 p-4">
  <section id="introPage" class=" grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class=" flex flex-col justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class=" font-semibold text-4xl sm:text-5xl md:text-6xl">
        We're <span class="poppins text-violet-400">MOUNT</span> CODE <br/>We build
        <span class="poppins text-violet-400">websites</span>
      </h2>
    <p class="text-base sm:text-lg md:text-xl">
      If you're not satisfied, <span class="poppins text-violet-400">100% money back guarantee</span>

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
    <img src="src/images/Mountcode-logo.png" alt="profile pic" class="object-cover z-[2] max-h-[70vh]" />

  </div>

  </section>

  <section id="projects" class=" py-20 lg:py-32 flex flex-col gap-24">
    <div class=" flex flex-col gap-2 text-center">
      <h6 class=" text-lg sm:text-xl md:text-2xl">A few of our creative endeavours</h6>
      <h3 class=" font-semibold text-3xl sm:text-4xl md:text-5xl">Curious to <span class="poppins text-violet-400">our</span> work? </h3>
      
    </div>
    <div class="flex flex-row justify-between">
      <a href="https://www.loom.com/share/a42dbce17933406d86a1780d61857038?sid=f86a6a4d-b4e6-4f8c-a6d2-6e0ade47d715&fbclid=IwAR3yeW1arS0NsQSP8hAEyxpPgs3FpuFV0MS4DlS1h8f9OiY7p4Eq9Rm5ys8" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>View Demo</p>
      </a>
      <a href="https://www.loom.com/share/bec45da26ecb4b42b82db4424e0dde43?fbclid=IwAR1IdJ6Pbqb2D_SKEOATlsJUJCim-fSfLT77B6gas8IfIasa9_fQFZNHe8Y" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>View Demo</p>
      </a>
      <a href="https://www.loom.com/share/74a4f5933d22468cad1c7bacad818e8d?sid=558ee602-4035-4c08-8d44-54ee55d8fe18&fbclid=IwAR0yvMlR_mRYSRGyoS64aF0FAB-w8E82XH2MxUFfDUk1cLEgFK-_3JH1Vjk" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>View Demo</p>
      </a>

    </div>
    <div class=" grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>Zez AI is an AI Image Generator.<strong class=" text-violet-400">You can create any image you want!</strong> First 5 images are FREE.
        </p>

      </Step>
      <Step step={steps[1]}>
        <p>Zez E-commerce is a digital image e-commerce store created to <strong class=" text-violet-400">showcase these cute lil wassies</strong> Seriously tho, how cute are they?
        </p>

      </Step>
      <Step step={steps[2]}>
        <p>Zez Jobs is a job marketplace. <strong class=" text-violet-400">Get the job of your dreams, if it even if exists.</strong> 
        </p>

      </Step>


    </div>

  </section>
  <section id="about" class=" py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div class=" flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
      <h6 class=" text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class=" font-semibold text-3xl sm:text-4xl md:text-5xl">A word <span class="poppins text-violet-400">from</span> the founder</h3>
    </div>
    <p class=" mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">Yoo, I'm Shaun. Long story short, I was an auditor at Deloitte, UK before co-founding an NFT project, which had a revenue of RM1.2 million. It was a ball of a time running it and I saw the power of tech and code, and thought it would be cool if I can empower retail businesses with this, starting with websites. Also, I a;ways believe in a win-win solution, so I only get paid if you're satisfied. 
    <!-- <div class=" flex justify-center items-center">
      <a href="/resume" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 w-80 hover:border-violet-700 duration-200">
        <p class="text-center ml-24">View Resume</p>
      </a>

    </div> -->
    <p class=" mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">Here's our pitch . . .

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
            <th class=" whitespace-nowrap p-2 px-4">Candidate #1

            </th>
            <th class=" whitespace-nowrap p-2 px-4">Candidate #2

            </th>
            <th class=" whitespace-nowrap p-2 px-4">Candidate #3

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
    <p class=" mx-auto">If you read till here, here's my present to you - have a good day :)</p>

  </section>

</main>
