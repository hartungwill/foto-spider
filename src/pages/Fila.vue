<template>
  <div class="q-px-lg q-pb-md">
    <q-timeline :layout="layout" color="secondary">
      <q-timeline-entry heading>
        Timeline heading
        <br>
        <!-- ({{$q.screen.lt.sm ? 'Dense' : ($q.screen.lt.md ? 'Comfortable' : 'Loose')}} layout) -->
      </q-timeline-entry>

      <q-timeline-entry
        title="Event Title"
        subtitle="February 22, 1986"
        side="right"
      >
        <q-card class="my-card">
          <!-- <q-card-section class="q-pt-none">
            <div>
              Lorem ipsum
            </div>
          </q-card-section> -->
          <q-card-section horizontal>
            <q-img
              class="col"
              src="https://cdn.quasar.dev/img/parallax2.jpg"
            />
            <q-card-actions vertical class="justify-around">
              <q-btn
              flat
              round
              color="red"
              icon="post_add"
              />
              <!-- <q-btn flat round color="accent" icon="bookmark" /> -->
              <q-btn
              flat
              round
              color="primary"
              icon="delete_outline"
              />
            </q-card-actions>
          </q-card-section>
        </q-card>
      </q-timeline-entry>

      <q-timeline-entry
        title="Event Title"
        subtitle="February 22, 1986"
        side="left"
      >
        <q-card class="my-card">
          <!-- <q-card-section class="q-pt-none">
            <div>
              Lorem ipsum
            </div>
          </q-card-section> -->
          <q-card-section horizontal>
            <q-img
              class="col"
              src="https://cdn.quasar.dev/img/parallax2.jpg"
            />
            <q-card-actions vertical class="justify-around">
              <q-btn
              flat
              round
              color="red"
              icon="post_add"
              />
              <!-- <q-btn flat round color="accent" icon="bookmark" /> -->
              <q-btn
              flat
              round
              color="primary"
              icon="delete_outline"
              />
            </q-card-actions>
          </q-card-section>
        </q-card>
      </q-timeline-entry>
    </q-timeline>
  </div>
</template>

<script>
export default {
  computed: {
    layout () {
      return this.$q.screen.lt.sm ? 'dense' : (this.$q.screen.lt.md ? 'comfortable' : 'loose')
    }
  }
}
</script>
