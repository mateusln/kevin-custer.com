<template>
  <section class="section">
    <div class="content has-text-centered">
      <figure class="image is-128x128" style="margin: auto">
        <g-image alt="Author image: Kevin Custer" class="is-rounded author__image" src="~/assets/images/author.jpg" width="180" height="180" blur="5" />
      </figure>

      <h1 class="title is-4 has-text-link">
        {{ $static.metadata.siteName }}
      </h1>

      <p class="subtitle is-6 has-text-grey-dark has-text-weight-medium">
        <strong>Software Engineer</strong><br/>
        Staunton, VA
      </p>

      <p class="subtitle is-7 has-text-grey-dark">
        I write about ServiceNow, Full-stack development, and more!
      </p>

      <p class="buttons is-centered">
        <b-tooltip type="is-black" 
                  label="Follow me on GitHub"
                  position="is-bottom">
          <a href="https://www.github.com/odinsride" 
             target="_blank" 
             aria-label="Link to Kevin Custer on Github (New Window)"
             rel="noopener"
          >
            <b-icon
              pack="fab"
              icon="github"
              size="is-large"
              type="is-dark"
            ></b-icon>
          </a>
        </b-tooltip>
      </p>
    </div>
  </section>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.author__image {
  box-shadow: 0px 2px 5px 2px rgba(0,0,0,0.4);
}

.buttons {
  margin-top: -0.3em;
}
</style>
