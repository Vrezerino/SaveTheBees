<!-- eslint-disable max-len -->
<template>
  <q-layout view='lHh Lpr lFf'>

    <q-header>
      <q-toolbar>
        <q-btn flat dense round icon='menu' aria-label='Menu' @click='toggleLeftDrawer' />
      </q-toolbar>
      <div class='q-px-lg q-pt-sm' style='font-family: Morison Bold Italic;'>
        <div :class="$q.screen.gt.sm ? 'text-h1' : 'text-h4'">Save The Bees</div>
        <div class='subtitle-1'>Information & Resources</div>
      </div>
      <div class='text-caption q-pr-sm' style='text-align: right;'>
        by <a href='https://github.com/Vrezerino' class='text-white ' style='text-decoration: none;'>
          Patrick Park
        </a>
      </div>
      <q-img src='/img/bee1.jpg' class='header-image absolute-top' />
    </q-header>

    <q-drawer v-model='leftDrawerOpen' show-if-above :width='250' :breakpoint='600'>
      <q-scroll-area style='height: calc(100% - 201px); margin-top: 201px; border-right: 1px solid #ddd'>
        <q-list padding>

          <q-item to='/' exact clickable v-ripple>
            <q-item-section avatar>
              <q-icon name='list' />
            </q-item-section>

            <q-item-section>
              How To Help
            </q-item-section>
          </q-item>

          <q-item to='/aboutbees' exact clickable v-ripple>
            <q-item-section avatar>
              <q-icon name='help' />
            </q-item-section>

            <q-item-section>
              About Bees
            </q-item-section>
          </q-item>
        </q-list>

      </q-scroll-area>

      <q-img class='corner-image absolute-top' src='/img/bees.jpg' style='height: 201px'>
        <div class='absolute-bottom bg-transparent'>
          <q-avatar size='56px' class='q-mb-sm'>
            <img src=''>
          </q-avatar>
          <div class='text-weight-bold'></div>
        </div>
      </q-img>
    </q-drawer>

    <q-page-container>
      <router-view v-slot='{ Component }'>
        <keep-alive>
          <component :is='Component' />
        </keep-alive>
      </router-view>
    </q-page-container>

  </q-layout>
</template>

<script setup>
import { ref } from 'vue';

defineOptions({
  name: 'MainLayout',
});

const leftDrawerOpen = ref(false);

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value;
}
</script>

<style lang='scss'>
.header-image {
  height: 100%;
  z-index: -1;
  opacity: 0.6;
  filter: grayscale(0%);
}

.corner-image {
  opacity: 1;
}
</style>
