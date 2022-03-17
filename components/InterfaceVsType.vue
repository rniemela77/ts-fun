<script setup lang="ts">
//-----------------Interface-----------------
// 1. Create interface
interface Animal1 {
  name: string;
}
// 2. Extend the interface
interface Bear1 extends Animal1 {
  honey: boolean;
}
// 3. Add a field to the interface `Bear1`
interface Bear1 {
  color?: string;
}
// 4. Set the var `bestBear1` to have the type <Bear1>
const bestBear1: Bear1 = { name: "Pooh", honey: true };

//-----------------Type-----------------
// 1. Create type
type Animal2 = {
  name: string;
};
// 2. Extend the type (via intersection)
type Bear2 = Animal2 & {
  honey: boolean;
};
// 3. Cannot add a field to a type!
// type Bear2 { ... }

// 4. Set the var `bestBear2` to have the type <Bear2>
const bestBear2: Bear2 = { name: "Pooh", honey: false };
</script>
