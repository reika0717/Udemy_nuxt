<template>
	<section class="post-list">
    <PostPreview 
      id="1"
      :is-admin="isAdmin"
      thumbnail="http://cryptotimes.org/wp-content/uploads/2018/06/050318_LRR_MEN_WomenTech.jpg"
      title="Hello there"
      previewText="This is my first post!"
    />
    <PostPreview 
      id="2"
      :is-admin="isAdmin"
      thumbnail="http://cryptotimes.org/wp-content/uploads/2018/06/050318_LRR_MEN_WomenTech.jpg"
      title="Hi"
      previewText="This is my second post!"
    />
    <PostPreview 
      id="3"
      :is-admin="isAdmin"
      thumbnail="http://cryptotimes.org/wp-content/uploads/2018/06/050318_LRR_MEN_WomenTech.jpg"
      title="I'm tired"
      previewText="This is my third post!"
    />
	</section>
</template>

<style scoped lang="sass">
	.post-page
		display: flex
		justify-content: center
		align-items: center

	.post-list
	  display: flex
	  padding: 20px
	  box-sizing: border-box
	  flex-wrap: wrap
	  align-items: center
	  justify-content: center
</style>

<script>
  import PostPreview from '@/components/Posts/PostPreview'

  export default {
    components: {
      PostPreview
    },
    props: {
      isAdmin: {
        type: Boolean,
        default: false
      }
    }
  }
</script>