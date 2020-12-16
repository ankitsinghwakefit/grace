<template>
<!-- <div>
  <div>
    <b-form-group
      id="fieldset-horizontal"
      label-cols-sm
      label-cols-md="2"
      label-cols-lg="1"
      label-cols-xl="1"
      
      content-cols-lg="1"
      content-cols-md="1"
      content-cols-xl="1"
      description="Let us know your name."
      label="Enter your name"
      label-for="input-horizontal"
    >
      <b-form-input id="input-horizontal"></b-form-input>
    </b-form-group>
  </div>
</div> -->
<div>
<div v-if="showForm">
  <div class="testing">
    <b-form-group
      id="fieldset-1"
      description="Let us know your name."
      label="Enter your name"
      label-for="input-1"
      valid-feedback="Thank you!"
      :invalid-feedback="invalidFeedback"
      :state="state"
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
        v-model="digits"
        :state="dig"
        trim
      ></b-form-input>
      
    </b-form-group>
    <b-form-textarea
      id="textarea"
      
      placeholder="Your Message..."
      rows="3"
      max-rows="6"
    ></b-form-textarea>
    <div class="tetsig4">
        <b-button v-on:click="displayForm" class="submitBtn" type="submit" variant="primary">Submit</b-button>
    </div>
    
  </div>
  </div>
  <div class="errorMsg">
    {{msg}}
  </div>
  </div>
</template>

<script>
export default {
  methods: {
    displayForm(){
      this.showForm = false;
      this.msg = "* Your network is not secure, Please try with safe connection or Call on above number"
    }
  },
  computed: {
    state() {
      return this.name.length >= 4;
    },
    dig() {
      return this.digits.length >= 9;
    },
    invalidFeedback() {
      if (this.name.length > 0) {
        return "Enter at least 4 characters.";
      }
      return "Please enter something.";
    },
    invalidDigits() {
      if (this.digits.length > 0) {
        return "Enter at least 10 digits.";
      }
      return "Please enter something.";
    }
  },
  data() {
    return {
      name: "",
      digits: "",
      showForm : true,
      msg: "",
    };
  }
};
</script>

<style scoped>
.testing {
    width: 40%;
    border: 1px solid #ab9856;
    border-radius: 8px;
    padding: 8px;
}
@media only screen and (max-width: 1000px) {
    .testing {
    width: 80%;
}
 }
 @media only screen and (max-width: 800px) {
    .testing {
    width: 90%;
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
  background-color: #AB9856;
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

.button span:after {
  content: '\00bb';
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
  box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24), 0 17px 50px 0 rgba(0,0,0,0.19);
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
    background-color: #AB9856;
    border-color: #AB9856;
    font-weight: bolder;
    color: #373445;
}
.errorMsg {
  color: rgb(204, 52, 52);
}
</style>
