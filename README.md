
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ngôi Nhà Kỷ Niệm</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #fffbf0;
        }
        .house {
            width: 300px;
            margin: 20px auto;
        }
        .floor {
            background: #ffcccb;
            border: 2px solid #d67b7b;
            padding: 10px;
            margin-bottom: 10px;
            cursor: pointer;
        }
        .garden {
            background: #c2f0c2;
            border: 2px solid #78c578;
            padding: 10px;
            cursor: pointer;
        }
        .content {
            display: none;
            background: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <h1>Ngôi Nhà Kỷ Niệm</h1>
    <div class="house">
        <div class="floor" onclick="toggleContent('floor1')">🏠 Tầng 1 - Kỷ Niệm Tuổi Thơ</div>
        <div class="floor" onclick="toggleContent('floor2')">🏠 Tầng 2 - Những Người Bạn</div>
        <div class="floor" onclick="toggleContent('floor3')">🏠 Tầng 3 - Ước Mơ Và Tương Lai</div>
        <div class="garden" onclick="toggleContent('garden')">🌳 Sân Vườn - Nơi Thư Giãn</div>
    </div>
    
    <div id="floor1" class="content">Nội dung về tuổi thơ của mày nè...</div>
    <div id="floor2" class="content">Viết về bạn bè, những người đã đến và đi...</div>
    <div id="floor3" class="content">Những giấc mơ, hoài bão trong tương lai...</div>
    <div id="garden" class="content">Sân vườn nơi thư giãn, chia sẻ cảm xúc...</div>

    <script>
        function toggleContent(id) {
            let contents = document.querySelectorAll('.content');
            contents.forEach(content => content.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }
    </script>
</body>
</html>
