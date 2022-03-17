<script setup lang="ts">
interface Point {
  x: number;
  y: number;
}

const printCoord = (pt: Point) => {
  console.log(pt.x, pt.y);
};

printCoord({ x: 25, y: 85 });
</script>
