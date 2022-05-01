<script>
  import { faAt } from "@fortawesome/free-solid-svg-icons/faAt";
  import { faCommentSms } from "@fortawesome/free-solid-svg-icons/faCommentSms";
  import { faGithub } from "@fortawesome/free-brands-svg-icons/faGithub";
  import { faLinkedin } from "@fortawesome/free-brands-svg-icons/faLinkedin";

  import Button from "../components/Button.svelte";
</script>

<div class="max-w-md m-auto text-center space-y-6 px-6 py-8">
  <h1 class="flex justify-center">
    <a href="https://whinfield.ltd">
      <img src="logo-black.png" alt="Whinfield LTD" class="w-[175px] lg:w-[250px]" />
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
      WHINFIELD LTD is a company registered in England and Wales owned and operated by ALEX
      WHINFIELD &copy; {new Date().getFullYear()}
    </p>
    <p class="flex flex-col space-x-2 justify-center space-y-1 lg:flex-row lg:space-y-0">
      <span>Company Number TBC00000</span>
      <span class="hidden lg:block">|</span>
      <span>VAT Number TBC000000</span>
    </p>
  </div>
</div>
