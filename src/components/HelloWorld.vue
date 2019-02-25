<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  created () {
    this.$fetch({
      api: 'internationCode'
    })
    this.$fetch({
      api: 'refund',
      params: {
        access_key: 'xu2I7vMfaqDfLm5n9uHXkp1zjWu8t1IQM9H4HUkeiEwBA8DF4Jft41E4Dt8mFEpp3WMTU9944J2X2K48TACjUtaOKdi38JOgCSjiiQ6H8Gew2iz5zy83P9U4',
        amount: '5',
        coin_name: 'BTC',
        user_type: 1
      }
    })
  },
  render () {
    return (
      <div>111</div>
    )
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
