<template>
  <div class="footer__container w-full md:pl-24 pl-0 mt-12 mb-4">
    <div class="footer__content lg:w-4/5 md:px-0 px-2 w-full mr-auto ml-auto">
      <div
        class="footer--text text-center border-b border-gray-100 p-8 md:text-2xl text-xl font-medium italic"
      >
        This project lives on donations. Consider
        <a href="https://paypal.me/deepjyoti30">donating</a> to help us sustain
        our activites or
        <a href="https://opencollective.com/ytmdl#backer">become a backer</a>.
      </div>
      <div
        class="footer--extra py-4 text-gray-500 text-center md:flex md:justify-between items-center block"
      >
        <div class="copyright--text lg:text-left">
          <span>© 2020-Present Ytmdl. All rights reserved.</span>
          <span class="lg:inline block md:mt-0 mt-2 md:ml-2 ml-0"
            ><a href="https://ytmdl.deepjyoti30.dev/terms"
              >Terms of Service</a
            ></span
          >
        </div>
        <div class="social--content md:mt-0 mt-6">
          <ul>
            <li>
              <a
                href="https://github.com/deepjyoti30/ytmdl-web-v2"
                title="GitHub"
              >
                <github-icon class="inline icon-up" />
              </a>
            </li>
            <li>
              <a href="https://t.me/ytmdl" title="Telegram">
                <send-icon class="inline icon-up" />
              </a>
            </li>
            <li>
              <a href="mailto:hello@deepjyoti30.dev" title="Mail">
                <mail-icon class="inline icon-up" />
              </a>
            </li>
            <li>
              <a href="https://twitter.com/DeepBarman30" title="Twitter">
                <twitter-icon class="inline icon-up" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { MailIcon, SendIcon, GithubIcon, TwitterIcon } from "vue-feather-icons";

export default {
  name: "Footer",
  components: { MailIcon, SendIcon, GithubIcon, TwitterIcon }
};
</script>

<style lang="scss" scoped>
.footer__container {
  .footer__content {
    .footer--text {
      a {
        color: $darkgreen;
        text-decoration: underline;
      }
    }

    .footer--extra {
      @extend .roboto;

      .social--content {
        ul {
          li {
            @apply inline-block;
            @apply mr-6;
          }

          li:last-child {
            @apply mr-0;
          }
        }
      }
    }
  }
}
</style>
