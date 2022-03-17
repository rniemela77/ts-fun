<script setup lang="ts">
const printId = (id: number | string) => {
  if (typeof id === "string") {
    console.log(id.toUpperCase());
  } else {
    console.log(id);
  }
};
printId(101); // ok
printId("202"); // ok
// printId({ myID: 22342 }); // ERROR

const welcomePeople = (x: string[] | string) => {
  if (Array.isArray(x)) {
    console.log("hello, ", x.join(" and "));
  } else {
    console.log("hello lone traveler ", x);
  }
};
</script>
