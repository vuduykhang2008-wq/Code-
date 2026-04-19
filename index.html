<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Giải đố cùng Kiều Nhi</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: #ffc0cb; /* Màu hồng sáng */
            font-family: 'Pacifico', cursive; /* Phông chữ Pacifico cho toàn bộ trang */
            overflow: hidden; /* Ẩn thanh cuộn */
            display: flex;
            flex-direction: column;
            align-items: center;
            height: 100vh;
        }

        /* --- Màn hình Load Trang (Overlay) --- */
        #load-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(180deg, #ffb6c1 0%, #ffc0cb 100%); /* Màu nền giống ảnh */
            z-index: 10000;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            transition: opacity 0.5s ease-out;
        }

        /* Container cho icon trôi nổi */
        #load-drifting-container {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 9999;
        }

        /* Icon trôi nổi chung */
        .drifting-icon {
            position: absolute;
            animation: drift linear infinite;
            z-index: 1;
            user-select: none; /* Không cho chọn text emoji */
        }

        /* Trái tim tải trang đập */
        #load-heart {
            animation: pulse 1s infinite alternate;
            margin-top: 50px;
            z-index: 10001;
            filter: drop-shadow(0 0 5px rgba(255, 255, 255, 0.7));
        }

        @keyframes pulse {
            0% { transform: scale(1); opacity: 1; }
            100% { transform: scale(1.15); opacity: 0.8; }
        }

        /* Văn bản tải mới */
        #load-text {
            color: white;
            font-size: 1.8rem;
            margin-top: 25px;
            z-index: 10001;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
            font-weight: bold;
        }

        /* Thanh loading chạy full */
        #load-progress-container {
            width: 80%;
            max-width: 300px;
            height: 6px;
            background-color: white;
            border-radius: 10px;
            margin-top: 20px;
            overflow: hidden;
            z-index: 10001;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        #load-progress-bar {
            width: 0%;
            height: 100%;
            background-color: #ff69b4; /* Hồng đậm cho loading bar */
            border-radius: 10px;
            transition: width 0.1s linear;
        }

        /* --- Nội dung chính --- */
        #main-content {
            display: none; /* Ban đầu ẩn */
            flex-direction: column;
            align-items: center;
            width: 100%;
            height: 100%;
            z-index: 1;
        }

        /* Container cho icon trôi nổi trong trang */
        #main-drifting-container {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 0;
        }

        h1 {
            color: #ff0000; /* Màu đỏ */
            font-size: 4rem;
            text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.8);
            margin-top: 8vh;
            text-align: center;
            z-index: 10;
        }

        .input-box {
            margin-top: 40px;
            display: flex;
            flex-direction: column;
            align-items: center;
            z-index: 10;
        }

        input {
            padding: 18px 30px;
            font-size: 1.3rem;
            color: #800080; /* Chữ màu tím */
            background-color: #f8e8f8;
            border: 3px solid #800080; /* Viền tím */
            border-radius: 35px;
            outline: none;
            width: 320px;
            text-align: center;
            box-shadow: 0 5px 10px rgba(128, 0, 128, 0.2);
            transition: all 0.3s ease;
            font-family: 'Pacifico', cursive; /* Áp dụng phông Pacifico cho ô nhập */
        }

        input:focus {
            box-shadow: 0 5px 18px rgba(128, 0, 128, 0.5);
            transform: scale(1.03);
        }

        button {
            margin-top: 20px;
            padding: 12px 35px;
            font-size: 1.3rem;
            color: white;
            background-color: #800080; /* Nút màu tím */
            border: none;
            border-radius: 25px;
            cursor: pointer;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
            font-family: 'Pacifico', cursive; /* Áp dụng phông Pacifico cho nút */
            transition: background-color 0.2s;
        }

        button:hover {
            background-color: #9932cc;
        }

        /* Ô kết quả duy nhất - Đã đổi sang phông chữ bình thường */
        #single-result-box {
            margin-top: 50px;
            width: 65px;
            height: 75px;
            background-color: white;
            border: 4px solid #ff1493;
            border-radius: 18px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 3.5rem;
            font-weight: bold;
            color: #ff1493;
            box-shadow: 0 8px 12px rgba(0,0,0,0.18);
            z-index: 10;
            filter: drop-shadow(0 0 3px rgba(255, 20, 147, 0.5));
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; /* Phông chữ in hoa bình thường */
        }

        p#feedback {
            margin-top: 25px;
            font-size: 1.3rem;
            color: #800080;
            font-weight: bold;
            height: 28px;
            z-index: 10;
        }

        /* Dãy trái tim nhỏ trôi nổi chậm rãi */
        #heart-drift-row {
            position: absolute;
            top: 20%;
            width: 100%;
            display: flex;
            justify-content: space-around;
            z-index: 0;
            overflow: hidden;
        }
        
        #heart-drift-row div {
            font-size: 1.2rem;
            color: #ff69b4;
            animation: drift linear infinite;
        }

        /* Hiệu ứng trôi nổi chậm chạp chung cho các icon */
        @keyframes drift {
            0% { transform: translate(0, 0) rotate(0deg); opacity: 0; }
            5% { opacity: 1; }
            50% { transform: translate(var(--random_x), var(--random_y)) rotate(360deg); opacity: 0.8; }
            95% { opacity: 1; }
            100% { transform: translate(var(--random_x), var(--random_y)) rotate(720deg); opacity: 0; }
        }

        /* Media Queries cho Mobile */
        @media (max-width: 600px) {
            h1 {
                font-size: 3rem;
                margin-top: 6vh;
            }

            input {
                width: 85%;
                font-size: 1.1rem;
                padding: 15px 25px;
                box-sizing: border-box;
            }

            button {
                font-size: 1.1rem;
                padding: 10px 30px;
            }

            #single-result-box {
                width: 55px;
                height: 65px;
                font-size: 2.8rem;
                border-width: 3px;
                border-radius: 15px;
            }

            p#feedback {
                font-size: 1.1rem;
            }
            
            #load-text {
                font-size: 1.4rem;
            }
        }
    </style>
</head>
<body>

    <div id="load-overlay">
        <div id="load-drifting-container"></div>

        <svg id="load-heart" viewBox="0 0 100 100" width="100" height="100">
            <path d="M50,15.7A31,31,0,0,1,81.3,47.1C81.3,73.5,50,90.4,50,90.4S18.7,73.5,18.7,47.1A31,31,0,0,1,50,15.7Z" fill="white" />
        </svg>
        
        <p id="load-text">đang gửi yêu thương đến em...</p>

        <div id="load-progress-container">
            <div id="load-progress-bar"></div>
        </div>
    </div>

    <div id="main-content">
        <div id="main-drifting-container"></div>
        
        <div id="heart-drift-row">
            <div style="animation-duration: 25s; animation-delay: 2s; left: 10%;">❤</div>
            <div style="animation-duration: 20s; animation-delay: 5s; left: 30%;">❤</div>
            <div style="animation-duration: 30s; animation-delay: 8s; left: 50%;">❤</div>
            <div style="animation-duration: 28s; animation-delay: 11s; left: 70%;">❤</div>
            <div style="animation-duration: 22s; animation-delay: 14s; left: 90%;">❤</div>
        </div>

        <h1>giải đố cùng Kiều Nhi</h1>

        <div class="input-box">
            <input type="text" id="keywordInput" placeholder="Nhập từ khóa bí mật...">
            <button onclick="checkKeyword()">Giải mã</button>
        </div>

        <p id="feedback"></p>

        <div id="single-result-box">
            <span>&nbsp;</span> </div>
    </div>

    <script>
        // --- Danh sách Emoji Mèo ---
        const catEmojis = [
            "🐱", "🐈", "🐈‍⬛", "😺", "😸", "😹", "😻", "🐱💖", "🐱💕", "🐱✨", "😼", "😏😺", "🐱😼", "🐱🔥", "😿", "😾", "🐱💔", "🐱🥀", "🙀", "😺❗", "😾❗", "😽", "😻", "💋🐱", "🐱💘", "🐱😘", "🐈‍⬛🌙", "🐱🌸", "🐱🎧", "🐱📷"
        ];

        // --- Hàm tạo icon trôi nổi ngẫu nhiên ---
        function createDriftingIcon(container, type = 'emoji') {
            const icon = document.createElement("div");
            icon.className = "drifting-icon";
            
            if (type === 'heart') {
                icon.innerText = "❤";
                icon.style.color = "#ff69b4"; // Hồng cho trái tim
                icon.style.fontSize = Math.random() * 0.5 + 0.8 + "rem"; // Nhỏ (0.8 - 1.3rem)
            } else {
                // Chọn ngẫu nhiên một emoji mèo
                icon.innerText = catEmojis[Math.floor(Math.random() * catEmojis.length)];
                icon.style.fontSize = Math.random() * 1.5 + 1.5 + "rem"; // Trung bình đến lớn (1.5 - 3rem)
            }
            
            // Vị trí ngẫu nhiên
            icon.style.left = Math.random() * 100 + "vw";
            icon.style.top = Math.random() * 100 + "vh"; // Bắt đầu ở bất cứ đâu
            
            // Thời gian di chuyển cực kỳ chậm chạp và ngẫu nhiên (10s đến 25s)
            icon.style.animationDuration = Math.random() * 15 + 10 + "s";
            icon.style.animationDelay = Math.random() * 5 + "s"; // Độ trễ ngẫu nhiên

            // Độ mờ ngẫu nhiên (0.5 đến 1)
            icon.style.opacity = Math.random() * 0.5 + 0.5;
            
            // Thiết lập random_x và random_y cho keyframes
            const randomX = (Math.random() * 60 - 30) + "vw"; // Di chuyển ngang -30 đến 30vw
            const randomY = (Math.random() * 60 - 30) + "vh"; // Di chuyển dọc -30 đến 30vh
            icon.style.setProperty('--random_x', randomX);
            icon.style.setProperty('--random_y', randomY);
            
            container.appendChild(icon);
            
            // Xóa icon sau khi di chuyển xong
            setTimeout(() => {
                icon.remove();
            }, 30000); 
        }

        // Tạo nhiều icon mèo trôi nổi cho màn hình Load
        const loadDriftingContainer = document.getElementById('load-drifting-container');
        for (let i = 0; i < 25; i++) { 
            createDriftingIcon(loadDriftingContainer);
        }

        // Tạo nhiều icon mèo và trái tim trôi nổi cho nội dung chính
        const mainDriftingContainer = document.getElementById('main-drifting-container');
        for (let i = 0; i < 30; i++) { 
            createDriftingIcon(mainDriftingContainer);
        }
        for (let i = 0; i < 15; i++) { 
            createDriftingIcon(mainDriftingContainer, 'heart');
        }

        // Tự động tạo trái tim trôi liên tục 
        setInterval(() => {
            createDriftingIcon(mainDriftingContainer, 'heart');
        }, 12000); 

        // Tự động tạo emoji mèo trôi liên tục
        setInterval(() => {
            createDriftingIcon(mainDriftingContainer);
        }, 8000); 

        // Tự động tạo icon cho load screen liên tục (cho đến khi ẩn)
        const loadDriftInterval = setInterval(() => {
            if (document.getElementById('load-overlay').style.display !== 'none') {
                createDriftingIcon(loadDriftingContainer);
            } else {
                clearInterval(loadDriftInterval);
            }
        }, 10000); 

        // --- JS cho Progress Bar ---
        let progress = 0;
        const progressBar = document.getElementById('load-progress-bar');
        const interval = setInterval(() => {
            progress += 1;
            progressBar.style.width = progress + '%';
            if (progress >= 100) {
                clearInterval(interval);
                // Sau khi full, chờ một chút rồi ẩn overlay
                setTimeout(() => {
                    document.getElementById('load-overlay').style.opacity = '0'; // Hiệu ứng mờ dần
                    setTimeout(() => {
                        document.getElementById('load-overlay').style.display = 'none';
                        document.getElementById('main-content').style.display = 'flex';
                    }, 500); // Đợi hiệu ứng mờ kết thúc
                }, 500);
            }
        }, 40); // Tốc độ tải, tổng cộng 4 giây cho 100%

        // --- Danh sách từ khóa và vị trí ký tự tương ứng ---
        const puzzleData = {
            "DETHUONG": { letter: "I" },
            "DANGYEU": { letter: "L" },
            "CUTE": { letter: "O" },
            "XYNHDEP": { letter: "V" },
            "KIEUNHI": { letter: "E" },
            "ANHYEUEM": { letter: "Y" },
            "ANHTHUONGEM": { letter: "O" },
            "ANHTHICHEM": { letter: "U" }
        };

        const resultBox = document.getElementById("single-result-box");

        function checkKeyword() {
            const inputField = document.getElementById("keywordInput");
            const feedback = document.getElementById("feedback");
            // Xóa dấu cách thừa và in hoa để dễ so sánh
            const keyword = inputField.value.trim().toUpperCase().replace(/\s+/g, '');

            if (puzzleData[keyword]) {
                const data = puzzleData[keyword];
                resultBox.innerHTML = data.letter; // Bỏ span chứa phông chữ Pacifico, dùng phông chữ in hoa bình thường của thẻ cha
                feedback.innerText = `Chính xác! Kiều Nhi giỏi quá! Đã mở khóa kí tự '${data.letter}'!`;
                feedback.style.color = "#800080";
                inputField.value = "";
            } else {
                feedback.innerText = "Sai rồi, Nhi thử lại nhé!";
                feedback.style.color = "#800080";
                resultBox.innerHTML = "<span>&nbsp;</span>"; // Xóa kí tự cũ
            }
        }

        // Bắt sự kiện nhấn Enter
        document.getElementById("keywordInput").addEventListener("keypress", function(event) {
            if (event.key === "Enter") {
                checkKeyword();
            }
        });

    </script>

</body>
</html>
