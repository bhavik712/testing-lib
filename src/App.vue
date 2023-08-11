<template>
  <form-input :fieldProperties="nameField"></form-input>
  <form-input :fieldProperties="emailField"></form-input>
</template>

<script>
import { FormInput } from "vue-component-lib";
import "vue-component-lib/style.css";
export default {
  name: "app",
  data() {
    return {
      emailField: {
        label: "Email",
        name: "userEmail",
        type: "email",
        placeholder: "Enter Your Email",
      },
      nameField: {
        label: "Name",
        name: "userName",
        type: "text",
        placeholder: "Enter Your Name",
      },
    };
  },
  components: {
    FormInput,
  },
};
</script>
