<script setup lang="ts">
type Point = {
  x: number;
  y: number;
};

const printCoord = (pt: Point) => {
  console.log(pt.x, pt.y);
};

printCoord({ x: 50, y: 25 });
</script>
