<template>
    <div id="app">
        <h1 class="header">{{ msg1 }}</h1>
        <h1 class="count">{{ msg2 }}</h1>
        <h1 class="footer">{{ msg3 }}</h1>
				<gismap></gismap>
    </div>
</template>

<script>
import gismap from './components/gis'
export default {
  name: 'App',
	components:{
    'gismap':gismap
  },
  data () {
    return {
      msg1: '首页的头部',
      msg2: '首页的内容部分',
      msg3: '首页的尾部'
    }
  }
}
</script>

<style>
    #app {
        width: 100%;
        height: 100%;
        background: #fafafa;
    }

    .header {
        width: 100%;
        height: 30%;
        background: #66ccff;
    }

    .count {
        width: 100%;
        height: 50%;
        background: yellow;
    }

    .footer {
        width: 100%;
        height: 20%;
        background: greenyellow;
    }
</style>
