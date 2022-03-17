<script setup lang="ts">
// Optional properties
const printName = (obj: { first: string; last?: string }) => {
  console.log(obj.first.toUpperCase);

  // console.log(obj.last.toUpperCase); <-- this results in TS error

  if (obj.last !== undefined) {
    // <-- this prevents TS error
    console.log("optional last name: ", obj.last.toUpperCase);
  }

  console.log(obj.last?.toUpperCase); // <-- this also prevents TS error
};

printName({ first: "q", last: "w" });
printName({ first: "q" });
</script>
