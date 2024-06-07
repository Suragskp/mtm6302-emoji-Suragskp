# mtm6302-emoji-Suragskp

Open your Floder where you want to clone and open git bash in that folder.
Command 1: git clone https://github.com/Suragskp/mtm6302-emoji-Suragskp.git
command 2: use cd command to get into the folder eg cd mtm6302-emoji-Suragskp
command 3: use "ls" command to check all the files.(you should get readme.md file)
command 4: use "touch index.html style.css script.js" (to make new file.)
command 5 use "ls" command to check all the files.(you should get readme.md, index.html style.css script.js files)
command 6: open vscode by command "code ."

![image](https://github.com/Suragskp/mtm6302-emoji-Suragskp/assets/169490774/709c7c38-a343-4d2e-8473-56de375833e1)

In your vscode open index.html and write the HTML code.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset = "UTF-8">
    <meta name ="viewport" content="width=device=width", initial-scale = 1.0">
    <title>Emoji Gallery</title>
    <link rel="stylesheet" href="style.css"
</head>
<body>
    <section id="emoji-gallery" class = "emoji-gallery"></section>
    <script src = "script.js"></script>
</body>
</html>

![image](https://github.com/Suragskp/mtm6302-emoji-Suragskp/assets/169490774/4614b241-e2ad-4f46-9db9-d6fc7ef43645)

Let us now code style.css
/*CSS Reset */
*{
    margin:0;
    padding:0;
    box-sizing: border-box;
}

body{
    font-family: Arial, sans-serif;
    display:flex;
    justify-content:center;
    align-items:center;
    min-height: 100vh;
    background-color: #f0f0f0;
}

.emoji-gallery{
    display: grid;
    grid-template-columns: repeat(auto-fill,minmax(100px, 1fr));
    gap: 10px;
    padding: 20px;
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

.emoji-item {
    text-align: center;
    padding: 10px;
    background-color: #fff;
    border : 1px solid #ddd;
    border-radius: 8px;
}

.emoji-item span{
    font-size:2rem;
}

.emoji-item code {
    display: block;
    margin-top: 5px;
    color: #555;
}
Output:

![image](https://github.com/Suragskp/mtm6302-emoji-Suragskp/assets/169490774/7f5d68aa-6fdb-401c-b632-f63711c2a32f)

now we will be doing script.js file

![image](https://github.com/Suragskp/mtm6302-emoji-Suragskp/assets/169490774/310a6d00-6f89-41a1-a7b2-bcf98faa1067)

document.addEventListener('DOMContentLoaded', () => {
    const emojis = [
        { code: '&#128512;', decimal: '128512' },
        { code: '&#128513;', decimal: '128513' },
        { code: '&#128514;', decimal: '128514' },
        { code: '&#128515;', decimal: '128515' },
        { code: '&#128516;', decimal: '128516' },
        { code: '&#128517;', decimal: '128517' },
        { code: '&#128518;', decimal: '128518' },
        { code: '&#128519;', decimal: '128519' },
        { code: '&#128520;', decimal: '128520' },
        { code: '&#128521;', decimal: '128521' },
        { code: '&#128522;', decimal: '128522' },
        { code: '&#128523;', decimal: '128523' }
    ];

    const emojiGallery = document.getElementById('emoji-gallery');

    emojis.forEach(emoji => {
        const emojiItem = document.createElement('div');
        emojiItem.classList.add('emoji-item');
        emojiItem.innerHTML = `
            <span>${emoji.code}</span>
            <code>${emoji.decimal}</code>
        `;
        emojiGallery.appendChild(emojiItem);
    });
});

output:

![image](https://github.com/Suragskp/mtm6302-emoji-Suragskp/assets/169490774/2460eaec-15e6-496b-8b34-0200f90c2fea)

once done save all the files and see the output




