<template>
  <div id="contactForm">
    <b-form @submit="onSubmit" @reset="onReset" v-if="show">
      <b-form-group
        id="input-group-1"
        label="Email address:"
        label-for="input-1"
        description="We'll never share your email with anyone else."
      >
        <b-form-input
          id="input-1"
          v-model="form.email"
          type="email"
          placeholder="Enter email"
          required
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-2" label="Your Name:" label-for="input-2">
        <b-form-input
          id="input-2"
          v-model="form.name"
          placeholder="Enter name"
          required
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-3" label="Food:" label-for="input-3">
        <b-form-select
          id="input-3"
          v-model="form.info"
          :options="info"
          required
        ></b-form-select>
      </b-form-group>
      <b-form-group>
        <b-form-textarea
          id="textarea"
          v-model="form.text"
          placeholder="Enter something..."
          rows="3"
          max-rows="3"
        ></b-form-textarea>
      </b-form-group>
      <b-button type="submit" variant="primary" class="formButton">Submit</b-button>
      <b-button type="reset" variant="danger" class="formButton">Reset</b-button>
    </b-form>
    <b-card class="mt-3" header="Form Data Result">
      <pre class="m-0">{{ form }}</pre>
    </b-card>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          email: '',
          name: '',
          info: null,
          checked: [],
          text: ''
        },
        info: [{ text: 'What do you need?', value: null }, 'Product', 'Support', 'Generall Question', 'Problem'],
        show: true
      }
    },
    methods: {
      onSubmit(event) {
        event.preventDefault()
        alert(JSON.stringify(this.form))
        window.open('mailto:test@example.com?subject='+ this.form.info +'&body='+ JSON.stringify(this.form))
      },
      onReset(event) {
        event.preventDefault()
        // Reset our form values
        this.form.email = ''
        this.form.name = ''
        this.form.info = null
        this.form.text = ''
        // Trick to reset/clear native browser form validation state
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>
<style lang="scss">
#contactForm{
  width: 80%; 
  margin: 10%;
  background-color: transparent;
  padding: 10px;
  border-radius: 5px;
  border: 0;
  -webkit-box-shadow: 5px 5px 19px 7px rgba(253,126,53,0.82); 
  box-shadow: 5px 5px 19px 7px rgba(62,90,121,0.82);
}
.formButton{
  margin-right: 1em;
}
</style>