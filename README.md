# lamvu59<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trang Web Của Tôi</title>
    <style>
        /* CSS Reset & Cơ bản */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f4f7f6;
            color: #333;
            line-height: 1.6;
        }

        /* Thanh điều hướng (Navbar) */
        nav {
            background: #2c3e50;
            color: #fff;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 1.5rem;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #3498db;
        }

        /* Phần Hero (Giới thiệu đầu trang) */
        header {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 60vh;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 1rem;
        }

        header h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        header p {
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
        }

        .btn {
            display: inline-block;
            background: #3498db;
            color: #fff;
            padding: 0.75rem 1.5rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            text-decoration: none;
            font-size: 1rem;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #2980b9;
        }

        /* Container nội dung */
        .container {
            max-width: 1100px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
            color: #2c3e50;
        }

        /* Các thẻ tính năng/dịch vụ */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .card {
            background: #fff;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            margin-bottom: 0.5rem;
            color: #3498db;
        }

        /* Chân trang (Footer) */
        footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 3rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }
            nav {
                flex-direction: column;
            }
            nav ul {
                margin-top: 1rem;
            }
        }
    </style>
</head>
<body>

    <!-- Thanh điều hướng -->
    <nav>
        <div class="logo">MyWebsite</div>
        <ul>
            <li><a href="#home">Trang chủ</a></li>
            <li><a href="#services">Dịch vụ</a></li>
            <li><a href="#about">Giới thiệu</a></li>
            <li><a href="#contact">Liên hệ</a></li>
        </ul>
    </nav>

    <!-- Phần banner chào mừng -->
    <header id="home">
        <h1>Chào mừng đến với Trang Web Của Tôi</h1>
        <p>Nơi chia sẻ kiến thức, dịch vụ và giải pháp công nghệ hàng đầu.</p>
        <button class="btn" onclick="sayHello()">Bắt đầu ngay</button>
    </header>

    <!-- Nội dung chính -->
    <div class="container" id="services">
        <h2 class="section-title">Dịch Vụ Nổi Bật</h2>
        <div class="grid">
            <div class="card">
                <h3>Thủ Công Web</h3>
                <p>Thiết kế website theo yêu cầu với giao diện đẹp mắt và tối ưu cho mọi thiết bị.</p>
            </div>
            <div class="card">
                <h3>Lập Trình App</h3>
                <p>Phát triển ứng dụng di động mượt mà trên cả hệ điều hành Android và iOS.</p>
            </div>
            <div class="card">
                <h3>Tối Ưu SEO</h3>
                <p>Giúp trang web của bạn đạt thứ hạng cao trên các công cụ tìm kiếm hàng đầu.</p>
            </div>
        </div>
    </div>

    <!-- Chân trang -->
    <footer>
        <p>&copy; 2026 MyWebsite. Bản quyền thuộc về tác giả.</p>
    </footer>

    <!-- JavaScript xử lý tương tác -->
    <script>
        function sayHello() {
            alert("Xin chào! Cảm ơn bạn đã ghé thăm trang web của tôi.");
        }
    </script>
</body>
</html>
