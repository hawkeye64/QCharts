<template>
  <q-page padding>
    <qcc-pie
      :data="data"
      :options="options" />
  </q-page>
</template>

<script>
import QccPie from 'quasar-ui-qcarboncharts/src/components/QccPie'
import 'quasar-ui-qcarboncharts/src/components/qcarboncharts.sass'

export default {
  components: {
    QccPie
  },
  setup() {
    const data = [
      {
        "group": "2V2N 9KYPM version 1",
        "value": 20000
      },
      {
        "group": "L22I P66EP L22I P66EP L22I P66EP",
        "value": 65000
      },
      {
        "group": "JQAI 2M4L1",
        "value": 75000
      },
      {
        "group": "J9DZ F37AP",
        "value": 1200
      },
      {
        "group": "YEL48 Q6XK YEL48",
        "value": 10000
      },
      {
        "group": "Misc",
        "value": 25000
      }
    ]

    const options = {
      "title": "Pie (centered)",
      "resizable": true,
      "legend": {
        "alignment": "center"
      },
      "pie": {
        "alignment": "center"
      },
      "height": "400px"
    }

    return {
      data,
      options
    }
  }
}
</script>
