<script>
  import { Link } from "svelte-routing";

  const nimLogo = "/android-chrome-512x512.png"

</script>

<svelte:head>
  <title>Nim Wiki - Apply</title>
</svelte:head>


<section class="relative flex h-screen bg-secondary-dark bg-no-repeat">
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

  <div class="container mx-auto grid justify-items-center max-h-1024-px">
    <h2 class="font-semibold text-4xl text-primary mt-48">
      Apply for a domain
    </h2>

    <div class="flex items-baseline">
      <span class="text-4xl text-primary mr-2">1.</span>
      <p class="text-2xl leading-relaxed text-white">
        First, make sure that the project you want to apply for is related to the 
        <a
          href="https://nim-lang.org/"
          class="text-primary font-bold"
          target="_blank"
        >
          nim programming language.
        </a>
        Libraries, projects and blogs would all be accepted. 
      </p>
    </div>

    <div class="flex items-baseline">
      <span class="text-4xl text-primary mr-2">2.</span>
      <p class="text-2xl leading-relaxed text-white">
        Next, if you do not have a GitHub Pages webpage, you can make one using the follwing link:  
        <a
          href="https://pages.github.com/"
          class="text-primary font-bold"
          target="_blank"
        >
          GitHub Pages.
        </a>
        If you do not want to use the nim documentation template, or want a head start on your page, you can use some of the provided website generators there.
      </p>
    </div>

    <div class="flex items-baseline">
      <span class="text-4xl text-primary mr-2">3.</span>
      <p class="text-2xl leading-relaxed text-white">
        Now you will need to determine your nim-wiki domain. Preferred choices are your GitHub username, or the libraries repository name (ex: 
                <a
          href="https://nim-lang.nim.wiki"
          target="_blank"
          class="text-primary font-bold"
        >
          nim-lang.nim.wiki
        </a>
        ). You will also need to get the link to your GitHub Pages webpage, and create a brief description of what you domain will include. Examples can be found on the 
        <Link to="/directory"
          class="text-primary font-bold"
        >
          directory page
        </Link>
        , or instructions can be found at the 
        <a
          href="https://github.com/isaacdonaldson/nim-wiki"
          class="text-primary font-bold"
          target="_blank"
        >
          nim-wiki
        </a>
        repository. Once you have created your GitHub Page and chosen a domain name, in Setting > Pages enter your chosen domain name and it will create the CNAME file for you. This is step is needed.
      </p>
    </div>

    <div class="flex items-baseline">
      <span class="text-4xl text-primary mr-2">4.</span>
      <p class="text-2xl leading-relaxed text-white">
        To apply for a new domain, you must go to the 
        <a
          href="https://github.com/isaacdonaldson/nim-wiki"
          class="text-primary font-bold"
          target="_blank"
        >
          nim-wiki repository
        </a>
        and open a pull request that adds your domain, link and description to the APPLICATIONS.md file. A 
        <a
          href="https://github.com/isaacdonaldson/nim-wiki/blob/main/APPLICATION_GUIDE.md"
          class="text-primary font-bold"
          target="_blank"
        >
          detailed guide
        </a>
        can be found, and will hopefully answer any questions. Once your pull request is merged, you can expect to see your domain working and in the directory fairly soon. If you have any questions you can reach me at 
                <a
          href="mailto:this@isaacdonaldson.com"
          class="text-primary font-bold"
          target="_blank"
        >
          this@isaacdonaldson.com
        </a>
      </p>
    </div>


    <div class="mt-12">
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
