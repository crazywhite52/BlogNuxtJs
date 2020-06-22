<template>
  <div>
    <b-form v-if="show">
      <b-form-group id="input-group-1" label="Email address:" label-for="input-1" description>
        <b-form-input
          id="input-1"
          v-model="form.username"
          type="email"
          required
          placeholder="Enter email"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-2" label="password:" label-for="input-2">
        <b-form-input
          id="input-2"
          type="password"
          v-model="form.password"
          required
          placeholder="Enter password"
        ></b-form-input>
      </b-form-group>

      <b-button @click="submitForm(form)" variant="primary">{{buttonText}}</b-button>
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
        username: 'whitemis@gmail.com',
        password: '123456789'
      },
      show: true
    }
  },
  props: ["submitForm","buttonText"],
  
}
</script>