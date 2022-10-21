# W3D_hw

<!DOCTYPE html>

<html>

<head>
<style>


</style>
</head>

<body> 
<script>

$('#bpp').click(
  function() {
    var v = new THREE.Vector3($('#vx'),$('#vy'),$('#vz'));
		var w = new THREE.Vector3($('#wx'),$('#wy'),$('#wz'));

		var dot = v.dot(w);
		var c = new THREE.Vextor3();
		c.crossVectors(v,w);
  }
);


$('#vw1').change( function() {
  dot = $(this).val();
});

$('#vw2x').change( function() {
  c.x = $(this).x.val();
});

$('#vw2y').change( function() {
  c.y = $(this).y.val();
});

$('#vw2z').change( function() {
  c.z = $(this).z.val();
});


</script>


<button id='bpp'> input OK</button> <br>
<div style="width:1000px;heitht:1000px;background:yellow;border:25px blue">
<p> v </p>
<hr>
x
<input type='text' id='vx' >
<br> y
<input type='text' id='vy'>
<br> z
<input type='text' id='vz' >
</div>
<div style="width:1000px;heitht:1000px;background:yellow;border:25px blue">
<p> w </p>
<hr>
x
<input type='text' id='wx' >
<br> y
<input type='text' id='wy'>
<br> z
<input type='text' id='wz' >
</div>

<div style="width:1000px;heitht:1000px;background:yellow;border:25px blue">
<p> inner product </p>
<hr>
v.w
<input type='text' id='vw1' >
<br>
<br>
<br>
<br> v X w
<hr>
x
<input type='text' id='vw2x'>
<br>y
<input type='text' id='vw2y'>
<br>z
<input type='text' id='vw2z'>
</div>

</body>

</html>
