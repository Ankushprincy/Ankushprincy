
   
```html
<!DOCTYPE html>
<html>
<head>
    <title>Popup Demo</title>
    <style>
        .popup {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: #3498db;
            padding: 20px;
            border-radius: 10px;
            color: white;
            text-align: center;
        }
        
        .options button {
            margin: 10px;
            padding: 5px 15px;
            background-color: #e74c3c;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <div class="popup" id="popup">
        <p>Bestie ji 🫴</p>
        <div class="options">
            <button id="yes">Yes</button>
            <button id="no">No</button>
        </div>
    </div>

    <script>
        const popup = document.getElementById('popup');
        const yesButton = document.getElementById('yes');
        const noButton = document.getElementById('no');

        yesButton.addEventListener('click', function() {
            const emojis = document.createElement('div');
            emojis.innerHTML = '😍🥰😘';
            emojis.style.fontSize = '50px';
            popup.appendChild(emojis);
        });

        noButton.addEventListener('click', function() {
            const blink = setInterval(function() {
                noButton.style.color = noButton.style.color === 'red' ? 'white' : 'red';
            }, 500);
            setTimeout(function() {
                clearInterval(blink);
                noButton.style.color = 'red';
            }, 5000);
        });
    </script>
</body>
</html
