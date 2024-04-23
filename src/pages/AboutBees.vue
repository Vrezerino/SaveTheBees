<template>
  <q-page class='q-pa-lg'>
    <h5 class='q-mt-none text-green' style='font-family: Morison Bold Italic;'>About Bees</h5>

    <div class='q-pb-xl' style='max-width: 200px'>
      <q-list dense bordered padding class='rounded-borders text-bold'>
        <q-item clickable v-ripple v-for='section in sections' :key='section.title'>
          <q-item-section>
            <router-link :to="{ path: 'aboutbees', hash: `#${section.title}` }">
              {{ section.title }}
            </router-link>
          </q-item-section>
        </q-item>
      </q-list>
    </div>

    <div class='content'>
      <div v-for='section in sections' :key="section.title + '.content'">
        <div :id='`${section.title}`' class='q-pa-sm q-mb-md bg-green'>
          <h5 class='q-ma-none text-white'>{{ section.title }}</h5>
        </div>
        <p class='q-mb-xl'>
          {{ section.content }}
        </p>
      </div>

      <div>Sources:</div>
      <ul>
        <li>
          <a href='https://www.nwf.org/Educational-Resources/Wildlife-Guide/Invertebrates/Bees' target='_blank'>
            https://www.nwf.org/Educational-Resources/Wildlife-Guide/Invertebrates/Bees
          </a>
        </li>
        <li>
          <a href='https://www.shopnwf.org/Garden-for-Wildlife/Observe-and-Learn/2780-NWF904S-Attracting-Birds-Butterflies-and-Other-Backyard-Wildlife.pro'
            target='_blank'>
            Mizejewski, David C. Attracting Birds, Butterflies and Other Backyard Wildlife.
            East Petersburg: Fox Chapel Publishing, 2004.
          </a>
        </li>
        <li>
          <a href='https://efotg.sc.egov.usda.gov/references/public/SC/Bee_Basics_North_American_Bee_ID.pdf'
            target='_blank'>
            Moisset, B., Buchmann, S. 2011. Bee Basics: An Introduction to Our Native Bees.
            USDA, Pollinator Partnership.
          </a>
        </li>
        <li>
          <a href='https://xerces.org/' target='_blank'>
            Xerces Society for Invertebrate Conservation
          </a>
        </li>
      </ul>
    </div>

  </q-page>
</template>

<script setup>
defineOptions({
  name: 'AboutPage',
});

const sections = [
  {
    title: 'Description',
    content: `Like all insects, a bee’s body is divided into three parts: a head with
        two antennae, a thorax with six legs, and an abdomen. All bees have
        branched hairs somewhere on their bodies and two pairs of wings. Only
        female bees have stingers (which are modified ovipositors, organs
        originally used to lay eggs). Many bee species have black and yellow
        coloration, but many do not—they actually come in a variety of
        colors, including green, blue, red, or black. Some are striped,
        and some even have a metallic sheen. They range in size from
        large carpenter bees and bumble bees to the tiny Perdita minima
        bee, which is less than two millimeters long.`,
  },
  {
    title: 'Range',
    content: `There are over 20,000 bee species worldwide, including the honey bee,
        which originated in Eurasia and has been imported around the globe as
        a domesticated species. Wild bees species live on every continent
        except Antarctica. In North America there are approximately 4,000
        native bee species occupying ecosystems from forests to deserts
        to grasslands.`,
  },
  {
    title: 'Diet',
    content: `Bees feed exclusively on sugary nectar and protein-rich pollen from
        flowering plants, unlike the carnivorous wasps from which they evolved.`,
  },
  {
    title: 'Behavior',
    content: `As they forage, bees perform the critical act of pollination. As a bee
        enters a flower to feed on nectar and gather pollen, some of the pollen
        sticks to the bee’s body. When the bee flies on, it deposits some of
        that pollen on the next flower it visits, resulting in fertilization,
        allowing the plant to reproduce and to generate the fruits and seeds
        so many other wildlife species rely on as a food source. In fact,
        bees pollinate a staggering 80 percent of all flowering plants,
        including approximately 75 percent of the fruits, nuts, and
        vegetables grown in the United States.

        Though all female bees can sting, they only do so when threatened.
        Honey bees, with hives filled with honey and larvae that need
        protecting, are generally more aggressive and likely to sting when
        disturbed than solitary native bees.`,
  },
  {
    title: 'Life History',
    content: `Bees begin life as eggs, which hatch into larvae the feed and pupate and
        eventually emerge in their adult form, where they visit flowers to feed
        on and gather nectar and pollen.

        Unlike the hive-forming domesticated honey bee or wild bumble bee species,
        most bees are solitary nesters. They don’t form hives, create honey, or
        live a communal lifestyle. Instead, they lay their eggs in a series of
        tiny chambers in tunnels in the ground, in hollow plant stems, or in
        decaying wood. Unlike hive-forming bee species, which collectively care
        for their young, female solitary bees provision their eggs with a ball
        of nectar and pollen and leave them to grow and pupate on their own
        with no parental care.

        However, some species do not build nests at all. These “cuckoo bees' will
        lay their eggs in nests built by other species. Cuckoo bees will sometimes
        kill the host species’ larvae to ensure their own eggs will have enough
        food to grow to adulthood.

        Queen bumble bees can live for a year and workers for a month. Solitary
        bees also live for about a year, with the majority of that time spent
        developing in their nesting chamber where they hatch, pupate, and often
        overwinter. Their adult lives, during which they are active, lasts
        approximately three to eight weeks. Females tend to live a bit longer,
        as they need to build a nest and lay eggs.`,
  },
  {
    title: 'Conservation',
    content: `Both domesticated honey bees and many native bee species are in decline.
        In fact some species, such as the once-common rusty patched bumblebee,
        are now listed as endangered in the U.S. Potential causes of these declines
        include habitat destruction, disease, agricultural and lawn and garden
        practices, use of pesticides, habitat fragmentation, changes in land
        use, invasive species, and climate change.

        Pollinators, notably native bees, are critical to the survival of
        plants, other wildlife, and people alike. The National Wildlife Federation
        maintains and supports several initiatives that support pollinators. Learn more
        about our work through Garden for Wildlife.`,
  },
  {
    title: 'Fun Fact',
    content: `Some species of bee employ a technique called sonication, or buzz pollination,
        when they harvest pollen. During sonication, the bee rapidly vibrates its
        flight muscles while attached to the flower. This loosens the pollen,
        which makes it easier to collect.`,
  },
  'Sources',
];
</script>

<style lang='scss'>
.content {
  max-width: 700px;
}
</style>
