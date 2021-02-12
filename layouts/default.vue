<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  head () {
    return {
      link: [
        //{ rel: 'stylesheet', href: 'https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css' }
      ],
      bodyAttrs: {
        //class: 'windows-scrollbar',
      },
      script: [
        { src: 'https://code.jquery.com/jquery-3.4.1.slim.min.js', body: true },
        { src: 'https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js', body: true },
        { src: 'https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js', body: true },
      ]
    }
  }
}
</script>
