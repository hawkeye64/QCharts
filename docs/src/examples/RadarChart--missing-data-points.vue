<template>
  <q-page padding>
    <qcc-radar
      :data="data"
      :options="options" />
  </q-page>
</template>

<script>
import QccRadar from 'quasar-ui-qcarboncharts/src/components/QccRadar'
import 'quasar-ui-qcarboncharts/src/components/qcarboncharts.sass'

export default {
  components: {
    QccRadar
  },
  setup() {
    const data = [
      {
        "group": "Sugar",
        "key": "London",
        "value": 25
      },
      {
        "group": "Oil",
        "key": "London",
        "value": 6
      },
      {
        "group": "Water",
        "key": "London",
        "value": 12
      },
      {
        "group": "Sugar",
        "key": "Milan",
        "value": 13
      },
      {
        "group": "Oil",
        "key": "Milan",
        "value": 6
      },
      {
        "group": "Water",
        "key": "Milan",
        "value": 28
      },
      {
        "group": "Sugar",
        "key": "Paris",
        "value": 19
      },
      {
        "group": "Oil",
        "key": "Paris",
        "value": 16
      },
      {
        "group": "Water",
        "key": "Paris",
        "value": 10
      },
      {
        "group": "Sugar",
        "key": "New York",
        "value": 11
      },
      {
        "group": "Oil",
        "key": "New York",
        "value": 18
      },
      {
        "group": "Water",
        "key": "New York",
        "value": 8
      },
      {
        "group": "Sugar",
        "key": "Sydney",
        "value": 12
      },
      {
        "group": "Oil",
        "key": "Sydney",
        "value": 16
      }
    ]

    const options = {
      "title": "Radar - Missing datapoints",
      "height": "400px"
    }

    return {
      data,
      options
    }
  }
}
</script>
