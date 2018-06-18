<template>
  <li :class="classList" @click="hideMobile" v-show='$can(getAcl)'>
    <slot></slot>
  </li>
</template>

<script>
export default {
  name: 'sidebar-nav-item',
  props: {
    classes: {
      type: String,
      default: ''
    },
    acl: {
      type: String,
      default: 'public'
    }
  },
  computed: {
    classList () {
      return [
        'nav-item',
        ...this.itemClasses
      ]
    },
    itemClasses () {
      return this.classes ? this.classes.split(' ') : ''
    },
    getAcl() {
      return this.acl
    }
  },
  methods: {
    hideMobile () {
      if (document.body.classList.contains('sidebar-show')) {
        document.body.classList.toggle('sidebar-show')
      }
    }
  }
}
</script>
