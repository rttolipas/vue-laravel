<template>
  <div class="row my-5">
    <div class="col-md-6 offset-md-3">
      <div class="card">
        <div class="card-body">
          <h4 class="text-center my-3">Signup</h4>
          <div class="form-group">
            <input v-model="name" type="text" name="name" placeholder="Name" class="form-control">
          </div>
          <div class="form-group">
            <input
              v-model="email"
              type="text"
              name="email"
              placeholder="Email"
              class="form-control"
            >
          </div>
          <div class="form-group">
            <input
              v-model="password"
              type="password"
              name="password"
              placeholder="Password"
              class="form-control"
            >
          </div>
          <div class="form-group">
            <button @click="registerUser" class="btn btn-success form-control">Signup</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      password: ""
    };
  },
  methods: {
    registerUser() {
      console.log(`${this.name} ${this.email} ${this.password}`);
    }
  }
};
</script>