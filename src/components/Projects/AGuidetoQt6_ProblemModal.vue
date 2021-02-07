<template>
  <div>
    <b-button id="learnMoreBt" v-b-modal.modal-prevent-closing>Have a Problem ?</b-button>
    <b-modal
      id="modal-prevent-closing"
      ref="modal"
      title="Do you have a Problem?"
      @show="resetModal"
      @hidden="resetModal"
      @ok="handleOk"
    >
      <form ref="form" @submit.stop.prevent="handleSubmit">
        <b-form-group
          label="Name"
          label-for="name-input"
          invalid-feedback="Name is required"
          :state="nameState"
        >
          <b-form-input
            id="name-input"
            v-model="name"
            :state="nameState"
            required
          ></b-form-input>
        </b-form-group>
        <b-form-group
          label="Your Problem"
          label-for="textarea"
          invalid-feedback="Message is requiered"
        >
          <b-textarea
            id="textarea"
            v-model="msg"
            required
          ></b-textarea>
        </b-form-group>
      </form>
    </b-modal>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        name: '',
        nameState: null,
        msg: '',
        submittedNames: []
      }
    },
    methods: {
      checkFormValidity() {
        const valid = this.$refs.form.checkValidity()
        this.nameState = valid
        return valid
      },
      resetModal() {
        this.name = ''
        this.msg = ''
        this.nameState = null
      },
      handleOk(bvModalEvt) {
        // Prevent modal from closing
        bvModalEvt.preventDefault()
        // Trigger submit handler
        this.handleSubmit()
      },
      handleSubmit() {
        // Exit when the form isn't valid
        if (!this.checkFormValidity()) {
          return
        }
        //send message to firebase
        console.log(this.name + this.msg)
        // Hide the modal manually
        this.$nextTick(() => {
          this.$bvModal.hide('modal-prevent-closing')
        })
      }
    }
  }
</script>
<style scoped>
#learnMoreBt{
  background-color: #FD7E35;
  color: black;
  font-weight: bold;
  font-size: 20px;
  margin-right: 1em;
  margin-bottom: 1em;
}
</style>