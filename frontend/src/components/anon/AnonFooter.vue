<template>
  <div class="anon-footer">
    <Content class="footer-contents">
      <b-row>
        <b-col cols="12" sm="6" md="4" lg="3">
          <h5>Kontakt</h5>
          <ul class="list-unstyled">
            <li><span class="font-weight-bold">Styret:</span> <a class="green-link" href="mailto:styret@nvdagen.no">styret@nvdagen.no</a></li>
            <li><span class="font-weight-bold">Bedrift:</span> <a class="green-link" href="mailto:bedrift@nvdagen.no">bedrift@nvdagen.no</a></li>
            <li><span class="font-weight-bold">Sponsor:</span> <a class="green-link" href="mailto:sponsor@nvdagen.no">sponsor@nvdagen.no</a></li>
          </ul>
        </b-col>

        <b-col cols="12" sm="6" md="4" lg="6" class="text-center">
          <h5>Nettverksdagen</h5>
          <p class="text-subtle">
            Nettverksdagen er en karrieremesse arrangert av studenter på studiet Kybernetikk og Robotikk ved NTNU.
            Hensikten er å gi studentene mulighet til å møte sine fremtidige arbeidsgivere,
            få informasjon om sommerjobber og et innblikk i arbeidslivet.
            Overskuddet fra dagen går til å finansiere en faglig ekskursjon til Asia.
          </p>
        </b-col>

        <b-col cols="12" sm="6" md="4" lg="3" class="text-right ">
          <h5>Følg oss</h5>
          <ul class="list-inline social-icons">
            <li class="list-inline-item">
              <a href="https://www.facebook.com/nvdagen">
                <font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook' }"/>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://www.linkedin.com/company/nettverksdagen-ntnu">
                <font-awesome-icon :icon="{ prefix: 'fab', iconName: 'linkedin' }"/>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://twitter.com/hashtag/nettverksdagen">
                <font-awesome-icon :icon="{ prefix: 'fab', iconName: 'twitter-square' }"/>
              </a>
            </li>
          </ul>
        </b-col>
      </b-row>
    </Content>
  </div>
</template>

<script>
import Content from '@/components/common/Content.vue'
import { library } from '@fortawesome/fontawesome-svg-core'
import { faFacebook, faLinkedin, faTwitterSquare } from '@fortawesome/free-brands-svg-icons'
library.add(faFacebook, faLinkedin, faTwitterSquare)
export default {
  name: 'AnonFooter.vue',
  components: {
    Content
  }
}
</script>

<style scoped lang="scss">
  .anon-footer {
    background: #122e2c;
    color: #fff;
    padding: 15px 0;
    .green-link {
      color: #388f89;
    }
    .text-subtle {
      color: #b7cdcb;
      font-weight:100;
    }
    .social-icons {
      font-size:25px;
      a {
        color:#fff;
      }
    }
  }
</style>
