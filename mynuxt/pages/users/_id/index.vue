<template>
    <div>
        <h1>This is single users ID : {{ $route.params.id }}</h1>
    </div>
</template>

<script>
export default {
  validate(data) {
      // console.log(data);
      // return data.params.id == 1;
      return /^\d+$/.test(data.params.id); // validate number only
  }
};
</script>
