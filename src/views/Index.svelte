<script>
  import { Link } from "svelte-routing";
  import TypeWriter from "components/Custom/TypeWriter.svelte"

  const domainNames = ['demo'];

  const nimLogo = "/android-chrome-512x512.png"
</script>

<svelte:head>
  <title>Nim Wiki</title>
</svelte:head>

<section class="header relative items-center flex h-screen bg-secondary-dark bg-no-repeat">
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
  <div class="container mx-auto items-center flex flex-wrap">
    <div class="w-full md:w-12/12 lg:w-12/12 xl:w-12/12 px-4">
      <div class="pt-32 sm:pt-0">
        <div class="md:w-8/12 lg:w-6/12 xl:w-6/12">
        <h2 class="font-semibold text-4xl text-primary">
          Nim Wiki - A place to host Nim project websites.
        </h2>
        <p class="mt-4 text-lg leading-relaxed text-white">
          Nim Wiki is a free place to host your project webpage. If you have a 
          <a
            href="https://pages.github.com/"
            class="text-primary font-bold"
            target="_blank"
          >
            GitHub Pages
          </a>
          for your Nim project, apply for a simple URL like one of the following:
        </p>
      </div>

        <div class="mt-4">
          <span class="flex flex-row text-secondary-dark text-4xl bg-primary rounded p-2">
          https://<TypeWriter classStyle="text-secondary-dark" words="{domainNames}"/>.nim.wiki
          </span>
        </div>

        <div class="mt-12">
          <Link to="/apply"
            class="text-secondary-dark font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-primary active:bg-yellow-200 hover:bg-yellow-200 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150"
          >
            Apply Now
          </Link>

          <a
            href="https://github.com/isaacdonaldson/nim-wiki"
            class="github-star ml-1 text-white font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-blueGray-700 active:bg-blueGray-600 hover:bg-blueGray-600 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150"
            target="_blank"
          >
            Github Project
          </a>

          <Link to="/directory"
            class="text-secondary-dark font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-primary active:bg-yellow-200 hover:bg-yellow-200 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150"
          >
          Directory
          </Link>
        </div>
      </div>
    </div>

  </div>
</section>
