<img id="galleryImage" src="photo1.jpg">

<button onclick="nextImage()">Next</button>

<script>
let images = ["photo1.jpg", "photo2.jpg", "photo3.jpg"];
let current = 0;

function nextImage() {
    current++;

    if (current >= images.length) {
        current = 0;
    }

    document.getElementById("galleryImage").src = images[current];
}
</script>
