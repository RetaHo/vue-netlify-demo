<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <div>Hello Word!</div>
  <div>Hello Word!</div>
  <div>Hello Word!</div>
  <div>Hello Word!</div>
  <div>Hello Word!</div>
  <div>Reta 你好！</div>
  <form name="Portfolio_Contact" 
      method="POST" 
      data-netlify="true"
      data-netlify-honeypot="bot-field" 
      data-netlify-recaptcha="true"
      action="/thank-you">
    <div className="form-group">
      <input
        type="text"
        name="name"
        placeholder="name"
        className="form-control"
      />
      <input
        type="email"
        placeholder="email"
        name="email"
        className="form-control"
      />
      <textarea
        name="message"
        rows="5"
        placeholder="message"
        className="form-control"
      ></textarea>
      <div data-netlify-recaptcha="true"></div>
    </div>
    <button type="submit" className="submit-btn btn" onClick={handleSubmit}>
      send me your message
    </button>
  </form>


  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
