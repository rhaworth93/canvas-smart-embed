# canvas-smart-embed

<div class="container123">
    <label for="textInput">Enter text:</label>
    <input type="text" id="textInput" placeholder="Enter text">
    <button type="button" onclick="updateText()">Add Text</button>
    <div id="master" aria-live="polite"></div>
</div>

<script>
function updateText() {
    const input = document.getElementById('textInput').value.trim();
    if (input) {
        document.getElementById('master').innerText = input;
    } else {
        alert("Please enter some text!");
    }
}
</script>
