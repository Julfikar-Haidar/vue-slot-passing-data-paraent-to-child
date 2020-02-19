<template>
  <div>
      <h1>Lorem ipsum dolor sit amet.</h1>
      <!-- {{message}} -->
      <!-- <slot name="para"></slot>
        <slot name="header"></slot> -->
        <form action="">
            <div id="form-header">
                <slot name="header"></slot>
            </div>
            <div id="form-body">
                <slot name="info"></slot>
            </div>
             <div id="form-button">
                <slot name="details"></slot>
            </div>
            <div id="form-footer">
                <slot name="footer"></slot>
            </div>
        </form>

  </div>
</template>

<script>


export default {
  name: 'student',
//   props: ['message']
}
</script>

<style>

</style>
