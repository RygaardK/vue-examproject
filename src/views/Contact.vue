<template>
  <div class="contact">
    <h2>Contact Page</h2>

    <div>
        <label for="message">Name</label>
        <input v-model="name" placeholder="Enter name">
        <p>Name is: {{ name }}</p>
    </div>
    
    <div>
        <label for="message">Message</label>
        <textarea v-model="message" placeholder="add multiple lines"></textarea>
        <p>Message is: {{ message }}</p>
    </div>
  </div>

</template>


<script>
export default {

}
</script>

<style>
.contact div {
    display: block;
    padding: 1em;
    margin: 1em;
    border: 1px solid black;
}
label {
    display: block;
}
.short {
    width:50%;
    margin-left:25%;
    margin-right:25%;
    margin-top: 1em;
    margin-bottom: 1em;
}
</style>