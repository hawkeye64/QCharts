<template>
  <q-page padding>
    <qcc-bar-simple
      :data="data"
      :options="options" />
  </q-page>
</template>

<script>
import QccBarSimple from 'quasar-ui-qcarboncharts/src/components/QccBarSimple'
import 'quasar-ui-qcarboncharts/src/components/qcarboncharts.sass'

export default {
  components: {
    QccBarSimple
  },
  setup() {
		const data = [
      {
        "group": "Qty",
        "value": 65000
      },
      {
        "group": "More",
        "value": 29123
      },
      {
        "group": "Sold",
        "value": 35213
      },
      {
        "group": "Restocking",
        "value": 51213
      },
      {
        "group": "Misc",
        "value": 16932
      }
    ]
    const options = {
      "title": "Vertical simple bar (discrete)",
      "axes": {
        "left": {
          "mapsTo": "value"
        },
        "bottom": {
          "mapsTo": "group",
          "scaleType": "labels"
        }
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
