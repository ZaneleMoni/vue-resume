<template>
  <section id="contact2">
    <h1>Contact</h1>
        <div class="underline"></div>
    <div class="contact">
      <div class="container">
        <div class="row" id="form">
          <div class="col" id="left">
            <div class="left-container">
              <div class="left-inner-container">
              </div>
              <div class="address">
                <div>
                  <i>email</i>
                  <p>zanelemoni4@gmail.com</p>
                </div>
                <div>
                  <i>phone</i>
                  <p>+27 62 433 4358</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="container">
              <form
                action="https://formspree.io/f/xlezjnoz"
                method="post"
                target="_blank" >
                <label> Name:</label>
                <input
                  name="name"
                  type="text"
                  required
                  v-model="name"
                  placeholder="Enter full name and surname"/>
                <label> Email:</label>
                <input
                  type="email"
                  required
                  v-model="email"
                  placeholder="Enter your email"/>

                <label> Number:</label>
                <input
                  type="text"
                  required
                  v-model="number"
                  placeholder="Enter your number"/>
                <div v-if="numberError" class="number">{{ numberError }}</div>
                
                <label for="inputMessage"> Message:</label>
                <textarea
                  class="form-control"
                  name="message"
                  id="inputMessage"
                  rows="5"
                  required
                >
                </textarea>
                <div class="terms">
                  <input type="checkbox" v-model="terms" required />
                  <label> Accept terms and conditions</label>
                </div>
                <div class="submit">
                  <button @click="submit">Submit</button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      number: "",
      role: "",
      terms: false,
      message: "",
      numberError: "",
    };
  },
  methods: {
    handleSubmit() {
      this.numberError =
        this.number.length > 9
          ? ""
          : "Number must be at least 10 characters long";
    },
    submit() {},
  },
};
</script>

<style scoped>

h1 {
  font-family: normal;
  padding-right: 100%;
}
.underline{
  background: linear-gradient(135deg, #e55d87 0%, #5fc3e4 100%);
  width: 70px;
  height: 2px;


}
#contact2 {
  background-color: #f5d3d559;
  padding-bottom: 80px;
  padding-top: 50px;
  font-size: 1.2em;
}
form {
  max-width: 50%;
  margin: 30px auto;
  background: rgb(185, 96, 96);
  text-align: left;
  padding: 20px;
  border-radius: 10px;
}
#form {
  background-color: white;
  border-radius: 10px;
  padding-bottom: 20px;
}
/* .h1,
h1 {
  text-align: center;
  color: gray;
  font-size: medium;
  padding-top: 1.5%;
} */
#contact2 {
  padding-left: 250px;
}
.col {
  height: 20%;
}
.address {
  display: flex;
}
.address i {
  font-size: 60px;
  padding: 165px;
}

label {
  color: rgb(12, 6, 6);
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}
.h2,
h2 {
  text-align: center;
  padding-bottom: 40px;
}

input,
select {
  display: block;
  padding: 10px 6px;
  width: 50%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  color: #555;
}

.number {
  color: yellow;
  margin-top: 10px;
  font-weight: bold;
}
form {
  height: 94%;
}
input[type="checkbox"] {
  display: inline-flex;
  width: 16px;
  margin: 0 10px 0 0;
  position: relative;
  top: 2px;
}
#message {
  height: 110px;
}
.left-inner-container {
  padding-top: 130px;
}
.contact {
  box-shadow: 20px;
}
button {
  background: white;
  border: 1px;
  float: right;
  padding-bottom: 20px;
  padding: 5px 15px;
  border-radius: 20px;
}
.submit {
  text-align: center;
}

@media screen and (max-width: 600px) {
  .address i {
    font-size: 60px;
    padding: 20px;
  }
  #contact2 {
    background-color: #f5d3d559;
    padding-bottom: 80px;
    padding-top: 30px;
    font-size: 1.2em;
  }
  .address i {
    display: none;
  }
  #left {
    display: none;
  }
  form {
    width: 100%;
  }
}
</style>
