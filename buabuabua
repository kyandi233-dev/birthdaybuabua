<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>神秘选妃仪式</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            background-color: #f4f5f7;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            color: #333;
        }

        .card {
            background-color: #ffffff;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
            width: 100%;
            max-width: 350px;
            text-align: center;
        }

        .birthday-greeting {
            font-size: 17px;
            font-weight: bold;
            color: #d9534f;
            margin-bottom: 20px;
            line-height: 1.5;
            padding-bottom: 20px;
            border-bottom: 2px dashed #eee;
        }

        .intro-text {
            font-size: 13px;
            color: #555;
            background-color: #f9f9f9;
            padding: 12px;
            border-radius: 8px;
            margin-bottom: 25px;
            line-height: 1.5;
            border-left: 4px solid #007bff;
            text-align: left;
            font-style: italic;
        }

        h2 {
            margin-top: 0;
            margin-bottom: 20px;
            font-size: 22px;
            font-weight: 600;
        }

        p {
            font-size: 16px;
            color: #666;
            margin-bottom: 15px;
        }

        select {
            width: 100%;
            padding: 12px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 8px;
            margin-bottom: 20px;
            background-color: #fff;
            outline: none;
            cursor: pointer;
            box-sizing: border-box;
        }

        select:focus {
            border-color: #007bff;
        }

        button {
            width: 100%;
            padding: 14px;
            font-size: 16px;
            color: #fff;
            background-color: #007bff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.2s;
            font-weight: 500;
        }

        button:hover {
            background-color: #0056b3;
        }

        button:disabled {
            background-color: #a0c4ff;
            cursor: not-allowed;
        }

        #result-box {
            display: none;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid #eee;
        }

        #result-box p {
            margin: 0 0 10px 0;
            color: #888;
        }

        #target-name {
            font-size: 26px;
            font-weight: bold;
            color: #d9534f;
            margin: 0;
        }
    </style>
</head>
<body>

    <div class="card">
        <div class="birthday-greeting">
            呱呱•史官•胡尔摩斯•胡总•舍长大人•胡紫淇 🍾生日快乐，恭喜奔二加入老登行列🎉 
        </div>

        <div class="intro-text">
            “这是一个紧张刺激的礼物赠送对象抽卡网页。为让每个人的生日能在同一天庆祝又完美地保护大家的钱包而制作。”
        </div>
        
        <h2>神秘选妃仪式</h2>
        <p>你系边个</p>

        <select id="user-select">
            <option value="" disabled selected>请选择...</option>
            <option value="0">蜈蚣</option>
            <option value="1">蝎子</option>
            <option value="2">壁虎</option>
            <option value="3">蟾蜍</option>
            <option value="4">毒蛇</option>
        </select>

        <button id="draw-btn" onclick="drawGift()">开始抽取</button>

        <div id="result-box">
            <p>你嘅女仔：</p>
            <h3 id="target-name"></h3>
        </div>
    </div>

    <script>
        const players = ["蜈蚣", "蝎子", "壁虎", "蟾蜍", "毒蛇"];

        function drawGift() {
            const selectBox = document.getElementById('user-select');
            const selectedIndex = selectBox.value;

            if (selectedIndex === "") {
                alert("请先选择你系边个！");
                return;
            }

            // 环形分配
            const targetIndex = (parseInt(selectedIndex) + 1) % players.length;
            const targetName = players[targetIndex];

            // 显示结果
            document.getElementById('result-box').style.display = 'block';
            document.getElementById('target-name').innerText = targetName;
            
            // 锁定按钮和下拉框
            selectBox.disabled = true;
            const btn = document.getElementById('draw-btn');
            btn.innerText = "抽取完成";
            btn.disabled = true;
        }
    </script>
</body>
</html>
