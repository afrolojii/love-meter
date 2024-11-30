function measureLove() {
    const name1 = document.getElementById('name1').value;
    const name2 = document.getElementById('name2').value;

    if (!name1 || !name2) {
        alert("Please enter both names!");
        return;
    }

    // Generate a random love percentage
    const lovePercentage = Math.floor(Math.random() * 101);

    // Randomly select a face
    const faces = ['😊', '😍', '😘', '😄', '😻', '💖', '💞', '💘'];
    const randomFace = faces[Math.floor(Math.random() * faces.length)];

    // Display the results
    document.getElementById('percentage').innerText = `${lovePercentage}%`;
    document.getElementById('face').innerText = randomFace;
}