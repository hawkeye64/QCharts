<template>
  <q-page padding>
    <qcc-scatter
      :data="data"
      :options="options" />
  </q-page>
</template>

<script>
import QccScatter from 'quasar-ui-qcarboncharts/src/components/QccScatter'

export default {
  components: {
    QccScatter
  },
  setup() {
    const data = [
      {
        "group": "Dataset 1",
        "employees": 5000,
        "sales": 32100
      },
      {
        "group": "Dataset 1",
        "employees": 3000,
        "sales": 25100
      },
      {
        "group": "Dataset 1",
        "employees": 8000,
        "sales": 12100
      },
      {
        "group": "Dataset 1",
        "employees": 4000,
        "sales": 53100
      },
      {
        "group": "Dataset 2",
        "employees": 5000,
        "sales": 32100
      },
      {
        "group": "Dataset 2",
        "employees": 2000,
        "sales": 34100
      },
      {
        "group": "Dataset 2",
        "employees": 4000,
        "sales": 23100
      },
      {
        "group": "Dataset 2",
        "employees": 7000,
        "sales": 14100
      },
      {
        "group": "Dataset 2",
        "employees": 6000,
        "sales": 53100
      }
    ]

    const options = {
      "title": "Scatter (linear x & y)",
      "axes": {
        "bottom": {
          "title": "No. of employees",
          "mapsTo": "employees",
          "scaleType": "linear"
        },
        "left": {
          "title": "Annual sales",
          "mapsTo": "sales",
          "scaleType": "linear"
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
