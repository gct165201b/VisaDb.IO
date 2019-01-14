<template>
  <div id="app">
    <Header />
    <FlightInfo />
    <SchemeInfo />
    <AboutVisa />
  </div>
</template>

<script>

import Header from './components/Header';
import FlightInfo from './components/FlightInfo';
import SchemeInfo from './components/SchemeInfo';
import AboutVisa from './components/AboutVisa';

export default {
  name: 'app',
  components: {
    Header,
    FlightInfo,
    SchemeInfo,
    AboutVisa
  }
}
</script>

<style>
  * {
    padding: 0;
    margin: 0;
  }

  body {
    font-family: 'Quicksand';
    line-height: 1.4;
    background: #f5f5f5;
  }

  a {
    text-decoration: none;
  }

  ul {
    list-style: none;
  }
</style>
