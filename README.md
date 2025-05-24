<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>

<body>
    <h1>Emoji Mood Toggle</h1>
    <img id="emoji" alt="mood emoji"
        src="https://emojiisland.com/cdn/shop/products/Unhappy_Face_Emoji_Icon_ios10_large.png?v=1571606093">
    <button id="toggle-btn">UnHappy</button>

    <script>
        const body = document.body;
        body.style.textAlign = "center";

        const img = document.getElementById("emoji");
        const toggle_btn = document.getElementById("toggle-btn");

        let isUnhappy = true;

        toggle_btn.addEventListener('click', () => {
            if (isUnhappy) {
                img.src = "https://creazilla-store.fra1.digitaloceanspaces.com/cliparts/65532/happy-emoji-clipart-md.png";
                toggle_btn.textContent = "Happy";
                img.style.height = "500px";
                img.style.width = "500px;"
            }
            else {
                img.src = "https://emojiisland.com/cdn/shop/products/Unhappy_Face_Emoji_Icon_ios10_large.png?v=1571606093"
                toggle_btn.textContent = "UnHappy";
                img.style.height = "500px";
                img.style.width = "500px;"

            }
            isUnhappy = !isUnhappy;
        })
    </script>
</body>

</html>
