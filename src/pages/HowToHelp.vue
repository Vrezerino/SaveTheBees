<template>
  <q-page class='q-pa-lg'>
    <h5 class='q-mt-none text-green' style='font-family: Morison Bold Italic;'>How To Help</h5>

    <!-- How To Help expander flex grid -->

    <div class='row'>
      <div class='col-sm-12 col-md-6'>
        <p class=''>
          Bees play a critical role in pollinating trees and flowers and maintaining
          healthy ecosystems. Honey bees alone pollinate 80 percent of all flowering
          plants, including more than 130 types of fruits and vegetables. Unfortunately,
          bee populations have dropped alarmingly, as have the populations of many
          other pollinator species.
        </p>

        <p class=''>
          Take the monarch as an example―the number of these iconic orange and black
          butterflies, renowned for their extraordinary annual migrations, has
          plummeted from one billion to only 34 million in the past 25 years.
        </p>

        <p class=''>
          The loss of pollinators is likely due to dwindling habitat, diseases, parasites,
          and environmental contaminants.
        </p>
      </div>
      <div class='col-sm-12 col-md-6'>
        <q-img :src='"/img/honeybee.jpg"' />
      </div>
    </div>

    <div class='row'>
      <div class='col-sm-12 col-md-6'>
        <q-img :src='"/img/Honey-Bees-on-Patterson-Lab-Roof-2048x1357.jpg"' class='gt-sm auto'/>
      </div>
      <div class='col-sm-12 col-md-6'>
        <!-- Padding, all sides, medium, on medium screens and larger only: -->
        <p class='q-pa-md-md'>
          Fortunately, you can help save the bees and encourage bee populations to thrive!
          There are a number of ways you can help them.

        <ul>
          <li>
            You can make yourself a "bee revival kit" and treat a tired bee with some sugar
            water, or you can buy such a kit from e.g.
            <a href='https://www.amazon.co.uk/Original-Bee-Revival-Kit-containing/dp/B08J81G68Y'
              target='_blank'>Amazon</a>,
            <a href='https://beevive.com/collections/bee-revival-kits' target='_blank'>Beevive</a>,
            or <a href='https://shop.wwf.org.uk/products/bee-revival-kit' target='_blank'>WWF</a>.
          </li>
          <li>
            Plant a range of flowers in your garden so bees have access to nectar from March
            to October.
          </li>
          <li>
            Eat sustainable, organic honey. Harmful chemicals are often used in agriculture
            to get rid of pests in our environment. Bees can pick up these insecticides when
            they are pollinating and take them back to the hive. This causes declines in the
            bee populations and can even make it into the honey we eat! If you choose to buy
            organic honey you are making sure that bees are pollinating in pesticide free areas.
          </li>
        </ul>

        To find localized information and more ways to help, use the expanders below.
        </p>
      </div>
    </div>

    <!-- Locale expander flex grid -->

    <div class='row q-col-gutter-xs' style='min-height: 600px'>
      <div class='col-xs-12 col-sm-12 col-md-3'>
        <div class='q-pt-md'>
          <q-list bordered class='rounded-borders'>
            <q-expansion-item expand-separator label='Asia'>

              <q-card>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_cn.jpg"' width='20px' />
                  China
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://www.earthshare.org/zh/13-simple-steps-to-save-the-bees/' target='_blank'>拯救蜜蜂的13个简单步骤</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_ind.jpg"' width='20px' />
                  India
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://www.nealsyard.co.jp/column/column/1069' target='_blank'>क्या हुआ जो मधुमक्खियां मर रही हैं</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_jp.jpg"' width='20px' />
                  Japan
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://www.nealsyard.co.jp/column/column/1069' target='_blank'>みつばちの危機を救おう</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_sk.jpg"' width='20px' />
                  South Korea
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://happybean.naver.com/donations/H000000190289?redirectYN=N' target='_blank'>해피빈</a>
                    </li>
                  </ul>
                </q-card-section>
              </q-card>
            </q-expansion-item>

          </q-list>
        </div>
      </div>
      <div class='col-xs-12 col-sm-12 col-md-3'>
        <div class='q-pt-md'>
          <q-list bordered class='rounded-borders'>
            <q-expansion-item expand-separator label='Europe'>

              <q-card>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_fin.jpg"' width='20px' />
                  Finland
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://www.mehilaiskummit.fi/mehilaistieto/' target='_blank'>Mehiläiskummit</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_fr.jpg"' width='20px' />
                  France
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://www.alveole.buzz/fr/ce-que-sauver-les-abeilles-veut-dire/' target='_blank'>Alvéole</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_ger.jpg"' width='20px' />
                  Germany
                  <ul class="q-pa-xs q-ma-xs q-ml-xl">
                    <li>
                      <a href='https://volksbegehren-artenvielfalt.de/' target='_blank'>Volksbegehren Artenvielfalt</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_ireland.jpg"' width='20px' />
                  Ireland
                  <ul>
                    <li>
                      <a href='https://pollinators.ie/communities/' target='_blank'>National Biodiversity Data
                        Centre</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_spain.jpg"' width='20px' />
                  Spain
                  <ul>
                    <li>
                      <a href='https://es.greenpeace.org/es/que-puedes-hacer-tu/peticiones/salvar-abejas/' target='_blank'>Greenpeace</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_swe.jpg"' width='20px' />
                  Sweden
                  <ul>
                    <li>
                      <a href='https://www.naturskyddsforeningen.se/kampanj/radda-bina/' target='_blank'>Naturskyddsföreningen</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_uk.jpg"' width='20px' />
                  United Kingdom
                  <ul>
                    <li>
                      <a href='https://www.wwf.org.uk/updates/our-tips-how-bee-friendly' target='_blank'>WWF</a>
                    </li>
                  </ul>
                </q-card-section>
              </q-card>
            </q-expansion-item>

          </q-list>
        </div>
      </div>
      <div class='col-xs-12 col-sm-12 col-md-3'>
        <div class='q-pt-md'>
          <q-list bordered class='rounded-borders'>
            <q-expansion-item expand-separator label='North America'>

              <q-card>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_canada.jpg"' width='20px' />
                  Canada
                  <ul>
                    <li>
                      <a href='https://beecitycanada.org/donate/' target='_blank'>Bee City Canada</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_us.jpg"' width='20px' />
                  United States
                  <ul>
                    <li>
                      <a href='https://www.treehugger.com/why-some-bees-endangered-and-what-we-can-do-5025654'
                        target='_blank'>Treehugger</a>
                    </li>
                    <li>
                      <a href='https://www.farmers.gov/blog/value-birds-and-bees' target='_blank'>USDA</a>
                    </li>
                  </ul>
                </q-card-section>
              </q-card>
            </q-expansion-item>

          </q-list>
        </div>
      </div>
      <div class='col-xs-12 col-sm-12 col-md-3'>
        <div class='q-pt-md'>
          <q-list bordered class='rounded-borders'>
            <q-expansion-item expand-separator label='Oceania'>

              <q-card>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_aus.jpg"' width='20px' />
                  Australia
                  <ul>
                    <li>
                      <a href='https://www.beethecure.com.au/' target='_blank'>Bee the Cure</a>
                    </li>
                  </ul>
                </q-card-section>
                <q-card-section class='q-pa-sm'>
                  <q-img :src='"/img/flags/flag_nz.jpg"' width='20px' />
                  New Zealand
                  <ul>
                    <li>
                      <a href='https://www.nzbct.org.nz/' target='_blank'>NZ Bumblebee Conservation Trust</a>
                    </li>
                  </ul>
                </q-card-section>
              </q-card>
            </q-expansion-item>

          </q-list>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
defineOptions({
  name: 'ResourcePage',
});
</script>
