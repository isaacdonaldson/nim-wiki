<script>
  import { Link } from "svelte-routing";

  const nimLogo = "/android-chrome-512x512.png"

</script>

<svelte:head>
  <title>Nim Wiki - Apply</title>
</svelte:head>


<section id="background-full" class="relative flex h-screen bg-secondary-dark bg-no-repeat">
  <a
    href="/"
    class="absolute top-0 left-0 max-w-150-px"
    style="margin-left: 50px; margin-top: 50px;"

  >
    <img
      src="{nimLogo}"
      alt="Nim Wiki Logo"
    />
  </a>

  <div class="container mx-auto grid justify-items-center max-h-1024-px p-4">
    <h2 class="font-semibold text-4xl text-primary mt-48 pt-8">
      Applying for a domain
    </h2>

    <div class="flex items-baseline mt-8">
      <span class="text-4xl text-primary mr-2">1.</span>
      <p class="text-2xl leading-relaxed text-white">
        Make sure that the project you want a domain for is related to the 
        <a
          href="https://nim-lang.org/"
          class="text-primary font-bold"
          target="_blank"
        >
          nim programming language.
        </a>
        Libraries, projects, or blogs would all be accepted. 
      </p>
    </div>

    <div class="flex items-baseline mt-8">
      <span class="text-4xl text-primary mr-2">2.</span>
      <p class="text-2xl leading-relaxed text-white">
        If you do not have a GitHub Pages webpage for your project, you will need to make one using the following link:  
        <a
          href="https://pages.github.com/"
          class="text-primary font-bold"
          target="_blank"
        >
          GitHub Pages.
        </a>
        The link also includes website generators if you do not want to use the nim documentation template, or want a head start on your webpage.
      </p>
    </div>

    <div class="flex items-baseline mt-8">
      <span class="text-4xl text-primary mr-2">3.</span>
      <p class="text-2xl leading-relaxed text-white">
        Select your nim-wiki domain. Preferred choices include your GitHub username, or the library repository name (<i>ex</i>. 
                <a
          href="https://demo.nim.wiki"
          target="_blank"
          class="text-primary font-bold"
        >
          demo.nim.wiki
        </a>). You will also need to get the link to your GitHub Pages webpage, and create a brief description of what your domain will include. Examples can be found on the 
        <Link to="/directory"
          class="text-primary font-bold"
        >
          directory page.
        </Link>
      </p>
    </div>

    <div class="flex items-baseline mt-8">
      <span class="text-4xl text-primary mr-2">4.</span>
      <p class="text-2xl leading-relaxed text-white">
        Enter your chosen domain name in your repository's Settings > Pages and it will create the CNAME file for you. Detailed instructions can be found in the 
        <a
          href="https://github.com/isaacdonaldson/nim-wiki/blob/main/APPLICATION_GUIDE.md"
          class="text-primary font-bold"
          target="_blank"
        >
          nim-wiki
        </a>
        application guide. This step is crucial.
      </p>
    </div>

    <div class="flex items-baseline mt-8">
      <span class="text-4xl text-primary mr-2">5.</span>
      <p class="text-2xl leading-relaxed text-white">
        To apply for the new domain, go to the 
        <a
          href="https://github.com/isaacdonaldson/nim-wiki"
          class="text-primary font-bold"
          target="_blank"
        >
          nim-wiki repository
        </a>
        and open a pull request that adds your domain, link and description to the APPLICATIONS.txt file. Once your pull request is merged, you can expect to see your domain working and in the directory fairly soon. A 
        <a
          href="https://github.com/isaacdonaldson/nim-wiki/blob/main/APPLICATION_GUIDE.md"
          class="text-primary font-bold"
          target="_blank"
        >
          detailed guide
        </a>
        can be found for all application steps, and will hopefully answer any questions. If you have any additional questions you can reach me at 
                <a
          href="mailto:this@isaacdonaldson.com"
          class="text-primary font-bold"
          target="_blank"
        >
          this@isaacdonaldson.com.
        </a>
      </p>
    </div>


    <div class="mt-12 pb-12">
          <Link to="/"
            class="text-secondary-dark font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-primary active:bg-yellow-200 hover:bg-yellow-200 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150"
          >
            Home
          </Link>
          <Link to="/directory"
            class="github-star ml-1 text-white font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-blueGray-700 active:bg-blueGray-600 hover:bg-blueGray-600 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150"
          >
            Directory
          </Link>
        </div>

  </div>
</section>
