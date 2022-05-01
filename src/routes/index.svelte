<script>
  import Fa from "svelte-fa";
  import { MetaTags } from "svelte-meta-tags";
  import { faAt } from "@fortawesome/free-solid-svg-icons/faAt";
  import { faCodeBranch } from "@fortawesome/free-solid-svg-icons/faCodeBranch";
  import { faCommentSms } from "@fortawesome/free-solid-svg-icons/faCommentSms";
  import { faGithub } from "@fortawesome/free-brands-svg-icons/faGithub";
  import { faLinkedin } from "@fortawesome/free-brands-svg-icons/faLinkedin";

  import Button from "../components/Button.svelte";

  const company = "Whinfield LTD";
</script>

<MetaTags
  title={`Alex Whinfield - Full Stack Software Development | ${company}`}
  canonical="https://whinfield.ltd/"
  openGraph={{
    url: "https://whinfield.ltd/",
    title: company,
    images: [
      {
        url: "https://www.whinfield.ltd/logo-black.png",
        width: 675,
        height: 552,
        alt: company
      }
    ],
    site_name: company
  }}
/>

<div class="max-w-md m-auto text-center space-y-6 px-6 py-8">
  <h1 class="flex justify-center">
    <a href="https://whinfield.ltd">
      <img src="logo-black.png" alt={company} class="w-[175px] lg:w-[250px]" />
    </a>
  </h1>
  <h2 class="text-2xl opacity-60 flex flex-col">
    <span>Alex Whinfield</span>
    <span class="block text-lg">Full Stack Software Development</span>
  </h2>
  <div
    class="flex flex-col space-x-0 justify-center space-y-2 lg:flex-row lg:space-y-0 lg:space-x-2"
  >
    <Button href="mailto:alex@whinfield.ltd" icon={faAt}>alex@whinfield.ltd</Button>
    <Button href="sms:+447414984753" icon={faCommentSms}>07414984753</Button>
    <Button href="https://github.com/alexwhin" icon={faGithub}>Github</Button>
    <Button href="https://www.linkedin.com/in/alexwhinfield/" icon={faLinkedin}>LinkedIn</Button>
  </div>
  <div class="opacity-40 text-sm space-y-2">
    <p>
      <span class="uppercase">{company}</span> is a company registered in England and Wales owned
      and operated by <span class="uppercase">Alex Whinfield</span> &copy; {new Date().getFullYear()}
    </p>
    <p class="flex flex-col space-x-2 justify-center space-y-1 lg:flex-row lg:space-y-0">
      <span>Company Number TBC00000</span>
      <a
        class="pt-1 opacity-70 hidden lg:block"
        href="https://github.com/alexwhin/whinfield.ltd"
        rel="noopener noreferrer"
        target="_blank"
        title="View on GitHub"
        ><Fa icon={faCodeBranch} />
      </a>
      <span>VAT Number TBC000000</span>
    </p>
  </div>
</div>
