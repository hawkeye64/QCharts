<template>
  <q-page padding>
    <qcc-bar-stacked
      :data="data"
      :options="options" />
  </q-page>
</template>

<script>
import QccBarStacked from 'quasar-ui-qcarboncharts/src/components/QccBarStacked'
import 'quasar-ui-qcarboncharts/src/components/qcarboncharts.sass'

export default {
  components: {
    QccBarStacked
  },
  setup() {
		const data = [
      {
        "group": "Dataset 1",
        "key": "Qty",
        "value": 65000
      },
      {
        "group": "Dataset 1",
        "key": "More",
        "value": 29123
      },
      {
        "group": "Dataset 1",
        "key": "Sold",
        "value": 35213
      },
      {
        "group": "Dataset 1",
        "key": "Restocking",
        "value": 51213
      },
      {
        "group": "Dataset 1",
        "key": "Misc",
        "value": 16932
      },
      {
        "group": "Dataset 2",
        "key": "Qty",
        "value": 32432
      },
      {
        "group": "Dataset 2",
        "key": "More",
        "value": 21312
      },
      {
        "group": "Dataset 2",
        "key": "Sold",
        "value": 56456
      },
      {
        "group": "Dataset 2",
        "key": "Restocking",
        "value": 21312
      },
      {
        "group": "Dataset 2",
        "key": "Misc",
        "value": 34234
      },
      {
        "group": "Dataset 3",
        "key": "Qty",
        "value": 12312
      },
      {
        "group": "Dataset 3",
        "key": "More",
        "value": 23232
      },
      {
        "group": "Dataset 3",
        "key": "Sold",
        "value": 34232
      },
      {
        "group": "Dataset 3",
        "key": "Restocking",
        "value": 12312
      },
      {
        "group": "Dataset 3",
        "key": "Misc",
        "value": 34234
      },
      {
        "group": "Dataset 4",
        "key": "Qty",
        "value": 32423
      },
      {
        "group": "Dataset 4",
        "key": "More",
        "value": 21313
      },
      {
        "group": "Dataset 4",
        "key": "Sold",
        "value": 64353
      },
      {
        "group": "Dataset 4",
        "key": "Restocking",
        "value": 24134
      },
      {
        "group": "Dataset 4",
        "key": "Misc",
        "value": 32423
      }
    ]
    const options = {
      "title": "Horizontal stacked bar (discrete)",
      "axes": {
        "left": {
          "scaleType": "labels",
          "mapsTo": "key"
        },
        "bottom": {
          "stacked": true,
          "mapsTo": "value"
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
