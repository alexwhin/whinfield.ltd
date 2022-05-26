<script>
  import Fa from "svelte-fa";
  import { faAt } from "@fortawesome/free-solid-svg-icons/faAt";
  import { faCodeBranch } from "@fortawesome/free-solid-svg-icons/faCodeBranch";
  import { faCommentSms } from "@fortawesome/free-solid-svg-icons/faCommentSms";
  import { faGithub } from "@fortawesome/free-brands-svg-icons/faGithub";
  import { faLinkedin } from "@fortawesome/free-brands-svg-icons/faLinkedin";

  import Logo from "../components/Logo.svelte";
  import Button from "../components/Button.svelte";
</script>

<div class="max-w-md m-auto text-center space-y-6 px-6 py-8">
  <h1 class="flex justify-center">
    <Logo />
  </h1>
  <h2 class="text-2xl opacity-60 flex flex-col">
    <span>Alex Whinfield</span>
    <span class="block text-lg">Full Stack Software &amp; Web Development</span>
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
      Whinfield LTD is a company registered in England and Wales, owned and operated by Alex
      Whinfield &copy;
      {new Date().getFullYear()}
    </p>
    <p class="flex flex-col space-x-2 justify-center space-y-1 lg:flex-row lg:space-y-0">
      <span>Company Number 14086093</span>
      <a
        class="pt-1 opacity-60 hidden lg:block"
        href="https://github.com/alexwhin/whinfield.ltd"
        rel="noopener noreferrer"
        target="_blank"
        title="View on GitHub"
        ><Fa icon={faCodeBranch} />
      </a>
    </p>
  </div>
</div>
