#Sample usage

Include `three.js` and `open-sans-light-typefacejs` in your HTML file:

    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r72/three.js"></script>
    <script src="bower_components/open-sans-light-typefacejs/open_sans_typeface.js"></script>

Then, a TextGeometry mesh that uses an Open Sans Light font can be added to a three.js `scene`:

    var shape = new THREE.TextGeometry("Hello, World!",
        {
            size: 60,
            height: 20,
            font: 'open sans light'
        });
    var wrapper = new THREE.MeshNormalMaterial({color: 0x00ff00});
    var words = new THREE.Mesh(shape, wrapper);
    scene.add(words);
