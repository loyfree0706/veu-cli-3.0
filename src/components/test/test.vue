<template>
<div>
    <div>
    <b-container fluid>
        <b-row class="text-center">
        <b-col xl="2" lg="3" md="4" sm="6" cols="12" class="py-3">
            <b-button v-b-popover.hover.top="'Popover!'" variant="primary">Top</b-button>
        </b-col>

        <b-col xl="2" lg="3" md="4" sm="6" cols="12" class="py-3">
            <b-button v-b-popover.hover.right="'Popover!'" variant="primary">Right</b-button>
        </b-col>

        <b-col xl="2" lg="3" md="4" sm="6" cols="12" class="py-3">
            <b-button v-b-popover.hover.left="'Popover!'" variant="primary">Left</b-button>
        </b-col>

        <b-col xl="2" lg="3" md="4" sm="6" cols="12" class="py-3">
            <b-button v-b-popover.hover.bottom="'Popover!'" variant="primary">Bottom</b-button>
        </b-col>

        <b-col xl="2" lg="3" md="4" sm="6" cols="12" class="py-3">
            <b-button v-b-popover.hover.bottom="'Popover!'" variant="primary">Bottom</b-button>
        </b-col>

        <b-col xl="2" lg="3" md="4" sm="6" cols="12" class="py-3">
            <b-button v-b-popover.hover.bottom="'Popover!'" variant="primary">Bottom</b-button>
        </b-col>
        </b-row>
    </b-container>
    </div>
</div>
</template>

<script>
  export default {
    data() {
      return {
        dismissSecs: 10,
        dismissCountDown: 0,
        showDismissibleAlert: false
      }
    },
    methods: {
      countDownChanged(dismissCountDown) {
        this.dismissCountDown = dismissCountDown
      },
      showAlert() {
        this.dismissCountDown = this.dismissSecs
      }
    }
  }
</script>