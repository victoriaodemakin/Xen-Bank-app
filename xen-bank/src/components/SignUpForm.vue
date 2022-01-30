<template>
  <form @submit.prevent="handleSumbit">
    <div class="input-container">
      <input
        class="input-field"
        type="email"
        required
        v-model="email"
        placeholder="Email"
        name="email"
      />
      <svg
        class="form-image"
        xmlns="http://www.w3.org/2000/svg"
        height="24px"
        viewBox="0 0 24 24"
        width="24px"
        fill="#FFFFFF"
      >
        <path d="M0 0h24v24H0V0z" fill="none" />
        <path
          d="M22 6c0-1.1-.9-2-2-2H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6zm-2 0l-8 5-8-5h16zm0 12H4V8l8 5 8-5v10z"
        />
      </svg>
    </div>

    <div class="input-container">
      <input
        class="input-field"
        type="text"
        v-model="name"
        placeholder="Name"
        name="name"
        required
      />
      <svg
        class="form-image"
        xmlns="http://www.w3.org/2000/svg"
        height="24px"
        viewBox="0 0 24 24"
        width="24px"
        fill="#FFFFFF"
      >
        <path d="M0 0h24v24H0V0z" fill="none" />
        <path
          d="M12 5.9c1.16 0 2.1.94 2.1 2.1s-.94 2.1-2.1 2.1S9.9 9.16 9.9 8s.94-2.1 2.1-2.1m0 9c2.97 0 6.1 1.46 6.1 2.1v1.1H5.9V17c0-.64 3.13-2.1 6.1-2.1M12 4C9.79 4 8 5.79 8 8s1.79 4 4 4 4-1.79 4-4-1.79-4-4-4zm0 9c-2.67 0-8 1.34-8 4v3h16v-3c0-2.66-5.33-4-8-4z"
        />
      </svg>
    </div>
    <div class="input-container">
      <select v-model="role">
        <option value="occupation">What you do</option>
        <option value="trader">Forex Trader</option>
        <option value="developer">Developer</option>
        <option value="banker">Banker</option>
      </select>
    </div>

    <button type="submit" class="form-btn">Join the Waiting List</button>
  </form>
</template>

<script>
export default {
  name: "SignUpForm",
  data() {
    return {
      email: "",
      name: "",
      role: "occupation",
    };
  },

  methods: {
    handleSubmit() {
      // validate password
      console.log("form submitted");
    },
  },
  props: ["name"],
};
</script>

<style>
.input-container {
  display: -ms-flexbox; /* IE10 */
  display: flex;
  width: 100%;
}
.form-image {
  position: relative;
  left: -30px;
  top: 20px;
}

input {
  width: 120%;
  padding: 1em;
  outline: white;
  margin: 1em 0;
  border: 1px solid var(--text-color);
  background: transparent;
  border-radius: 5px;
  color: var(--text-color);
}
select {
  width: 95%;
  padding: 1em;
  outline: white;
  margin: 1em 0;
  border: 1px solid var(--text-color);
  background: transparent;
  border-radius: 5px;
  color: var(--text-color);
}
::-webkit-input-placeholder {
  color: var(--text-color);
  transition: opacity 0.3s ease-in-out;
}
focus::-webkit-input-placeholder {
  opacity: 0.5s;
}

.input-field:focus {
  border: 1px solid var(--text-color);
}
select:focus {
  border: 1px solid var(--text-color);
}
/* Set a style for the submit button */
.form-btn {
  background-color: #0066cc;
  color: white;
  padding: 15px 20px;
  border: none;
  cursor: pointer;
  width: 200px;
  opacity: 0.9;
  margin: 1em 15%;
}

.btn:hover {
  opacity: 1;
}
</style>
