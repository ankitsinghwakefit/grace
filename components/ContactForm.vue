<template>
  <div>
    <!-- <div v-if="showForm">
  <div class="testing">
    <b-form-group
      id="fieldset-1"
      description="Let us know your name."
      label="Enter your name"
      label-for="input-1"
      valid-feedback="Thank you!"
      :invalid-feedback="invalidFeedback"
      :state="state"
      v-model="name"
    >
      <b-form-input
        id="input-1"
        v-model="name"
        :state="state"
        trim
      ></b-form-input>
    </b-form-group>
    <b-form-group
      id="fieldset-2"
      description="Let us know your digits."
      label="Enter your digits"
      label-for="input-2"
      valid-feedback="Thank you!"
      :invalid-feedback="invalidDigits"
      :state="dig"
    >
      <b-form-input
        id="input-2"
        v-model="number"
        :state="dig"
        trim
      ></b-form-input>
      
    </b-form-group>
    <b-form-textarea
      id="textarea"
      v-model="msg"
      placeholder="Your Message..."
      rows="3"
      max-rows="6"
    ></b-form-textarea>
    <div class="tetsig4">
      
        <b-button  class="submitBtn" type="submit" ><a target="_blank" href="https://forms.gle/TWodrXiE7uF5crmWA">Submit</a></b-button>
    </div>
    
  </div>
  </div> -->
    <div>
      <b-form @submit="onSubmit">
        <b-form-group id="input-group-1" label="Name:" label-for="input-1">
          <b-form-input
            id="input-1"
            v-model="form.name"
            type="text"
            placeholder="Enter Name"
            required
          ></b-form-input>
        </b-form-group>

        <b-form-group
          id="input-group-2"
          label="Your Number:"
          label-for="input-2"
        >
          <b-form-input
            id="input-2"
            v-model="form.number"
            type="number"
            placeholder="Enter Number"
            required
          ></b-form-input>
        </b-form-group>

        <b-form-group
          id="input-group-3"
          label="Your Msg:"
          label-for="textarea"
        >
        <b-form-textarea
        
          id="textarea"
          v-model="form.msg"
          placeholder="Enter your Msg..."
          rows="3"
          max-rows="6"
        ></b-form-textarea></b-form-group>

        <b-button class="mt-4" type="submit" variant="primary">Submit</b-button>
      </b-form>
    </div>
  </div>
</template>

<script>
const axios = require("axios");
export default {
  data() {
    return {
      form: {
        name: "",
        number: "",
        msg: ""
      }
    };
  },
  methods: {
    onSubmit(event) {
      event.preventDefault();
      alert(JSON.stringify(this.form));
      console.log(this.form);
      axios
        .post("https://muktiv2.herokuapp.com/", {
          name: this.form.name,
          number: this.form.number,
          msg: this.form.msg
        })
        .then(function(response) {
          console.log(response);
        })
        .catch(function(error) {
          console.log(error);
        });
    }
  }
};

// computed: {
//   state() {
//     return this.name.length >= 4;
//   },
//   dig() {
//     return this.number.length >= 9;
//   },
//   invalidFeedback() {
//     if (this.name.length > 0) {
//       return "Enter at least 4 characters.";
//     }
//     return "Please enter something.";
//   },
//   invalidDigits() {
//     if (this.number.length > 0) {
//       return "Enter at least 10 digits.";
//     }
//     return "Please enter something.";
//   }
// },
// data() {
//   return {
//     name: "",
//     number: "",
//     msg: ""
//   };
// },
// methods: {
//   displayForm() {
//     this.showForm = false;
//     this.msg =
//       "* Your network is not secure, Please try with safe connection or Call on above number";
//   },
//   formSubmitted() {
//     console.log("testing", name);
//   }
// }
</script>

<style scoped>
.testing {
  width: 100%;
  border: 1px solid #ab9856;
  border-radius: 8px;
  padding: 8px;
}
@media only screen and (max-width: 1000px) {
  .testing {
    width: 100%;
  }
}
@media only screen and (max-width: 800px) {
  .testing {
    width: 100%;
  }
}
@media only screen and (max-width: 750px) {
  .testing {
    width: 100%;
  }
}
.button {
  display: inline-block;
  border-radius: 13px;
  background-color: #ab9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 250px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}
a {
  color: #373445;
}

.button span:after {
  content: "\00bb";
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
button:hover {
  box-shadow: 0 12px 16px 0 rgba(0, 0, 0, 0.24),
    0 17px 50px 0 rgba(0, 0, 0, 0.19);
}
.tetsig4 {
  display: flex;
  width: 100%;
  justify-content: center;
  align-items: center;
  margin: 13px;
}
.submitBtn {
  width: 160px;
  background-color: #ab9856;
  border-color: #ab9856;
  font-weight: bolder;
  color: #373445;
}
.errorMsg {
  color: rgb(204, 52, 52);
}
</style>
