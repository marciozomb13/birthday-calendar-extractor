<template>
  <tr>
    <td>{{item.name}}</td>
    <td>{{item.start}}</td>
    <td>{{item.href}}</td>
    <td>DAY</td>
    <td>WEEK</td>
  </tr>
</template>

<script lang="ts">
  import Vue from 'vue';
  import Component from 'vue-class-component';

  const Props = Vue.extend({
    props: {
      item: {},
    },
  });

  // The @Component decorator indicates the class is a Vue component
  @Component
  export default class BirthdayRow extends Props {
    item: {
      name: string;
      start: string;
      href: string;
    };
  }
</script>
