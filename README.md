<!DOCTYPE html>
<html lang="he">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>צ'אט בוט</title>
    <style>
        /* סגנונות לתמונה ברקע */
        body {
            margin: 0;
            padding: 0;
            height: 100vh;
            background-image: url('YOUR_IMAGE_URL_HERE'); /* הכנס את הקישור לתמונה */
            background-size: cover;
            background-position: center;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        /* סגנונות לצ'אט-בוט */
        #chat-container {
            position: absolute;
            bottom: 20px;
            left: 20px;
            right: 20px;
            height: 500px;
            width: 100%;
            max-width: 400px;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 8px;
            overflow: hidden;
        }

        /* אם יש צורך להוסיף סגנונות נוספים לצ'אט-בוט */
        iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
    </style>
</head>
<body>

    <!-- מיכל הצ'אט-בוט -->
    <div id="chat-container">
        <script type="text/javascript">
            (function(d, t) {
                var v = d.createElement(t), s = d.getElementsByTagName(t)[0];
                v.onload = function() {
                    window.voiceflow.chat.load({
                        verify: { projectID: '674caacf1f89e3926fa903ad' },
                        url: 'https://general-runtime.voiceflow.com',
                        versionID: 'production'
                    });
                }
                v.src = "https://cdn.voiceflow.com/widget/bundle.mjs"; 
                v.type = "text/javascript"; 
                s.parentNode.insertBefore(v, s);
            })(document, 'script');
        </script>
    </div>

</body>
</html>
