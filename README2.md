<div class="header">
        <h1>Termux XMRig Miner - Đào Monero tự động trên Android</h1>
        <div class="badges">
            <span class="badge" style="background-color: #3498db;">Platform: Termux</span>
            <span class="badge" style="background-color: #27ae60;">Language: Bash</span>
            <span class="badge" style="background-color: #9b59b6;">License: MIT</span>
        </div>
        <img src="https://i.imgur.com/JqYe3Wn.png" alt="XMRig Miner Screenshot" class="center-img" width="400">
    </div>

    <div class="section">
        <h2 class="section-title">📌 Giới thiệu</h2>
        <p>Một script tự động hóa quá trình đào Monero (XMR) trên thiết bị Android thông qua Termux sử dụng XMRig.</p>
    </div>

    <div class="section">
        <h2 class="section-title">🌟 Tính năng nổi bật</h2>
        <div class="feature-box">
            <ul>
                <li>✅ Tự động cài đặt XMRig và các dependencies cần thiết</li>
                <li>✅ Menu điều khiển trực quan với các tùy chọn:
                    <ul>
                        <li>Bắt đầu đào Monero</li>
                        <li>Cập nhật XMRig phiên bản mới nhất</li>
                        <li>Xem giá XMR theo thời gian thực</li>
                    </ul>
                </li>
                <li>✅ Kiểm tra kết nối mạng tự động trước khi đào</li>
                <li>✅ Hiển thị thông tin hệ thống với neofetch</li>
                <li>✅ Hỗ trợ cả thiết bị ARM và x86</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2 class="section-title">🛠️ Yêu cầu hệ thống</h2>
        <ul>
            <li>Thiết bị Android 7.0 trở lên</li>
            <li>Termux phiên bản mới nhất</li>
            <li>Kết nối Internet ổn định</li>
            <li>Tối thiểu 2GB RAM (khuyến nghị 4GB+)</li>
            <li>Pin dung lượng lớn hoặc cắm sạc khi đào</li>
        </ul>
    </div>

    <div class="section">
        <h2 class="section-title">📥 Cài đặt</h2>
        <div class="code-block">
            # Cập nhật hệ thống và cài đặt công cụ cần thiết<br>
            pkg update -y && pkg upgrade -y<br>
            pkg install git cmake -y<br><br>
            
            # Clone repository<br>
            git clone https://github.com/d4m-dev/Xmrig.git<br>
            cd Xmrig<br><br>
            
            # Cấp quyền thực thi<br>
            chmod +x xmrig-menu.sh<br><br>
            
            # Chạy chương trình<br>
            ./xmrig-menu.sh
        </div>
    </div>

    <div class="section">
        <h2 class="section-title">🚀 Cách sử dụng</h2>
        <p>Sau khi chạy script, bạn sẽ thấy menu chính:</p>
        <div class="code-block">
            =================================<br>
               TERMUX XMRIG MINER - v1.0<br>
            =================================<br>
            1. Bắt đầu đào Monero<br>
            2. Cập nhật XMRig<br>
            3. Xem giá XMR hiện tại<br>
            4. Thông tin hệ thống<br>
            5. Thoát<br>
            =================================
        </div>
        <p>Chọn số tương ứng với chức năng bạn muốn sử dụng.</p>
    </div>

    <div class="section">
        <h2 class="section-title">⚠️ Lưu ý quan trọng</h2>
        <div class="warning-box">
            <strong>⚠️ Cảnh báo:</strong>
            <ul>
                <li>Đào tiền ảo có thể làm nóng thiết bị và giảm tuổi thọ pin</li>
                <li>Một số nhà mạng/dịch vụ có thể chặn kết nối mining</li>
                <li>Hiệu suất đào trên điện thoại thấp hơn nhiều so với máy tính</li>
                <li>Luôn theo dõi nhiệt độ thiết bị khi đào</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2 class="section-title">🔄 Cập nhật phiên bản mới</h2>
        <div class="code-block">
            cd ~/Xmrig<br>
            git pull origin main<br>
            chmod +x xmrig-menu.sh<br>
            ./xmrig-menu.sh
        </div>
    </div>

    <div class="section">
        <h2 class="section-title">📊 Hiệu suất dự kiến</h2>
        <table>
            <tr>
                <th>Thiết bị</th>
                <th>Hashrate (H/s)</th>
                <th>Nhiệt độ</th>
            </tr>
            <tr>
                <td>Snapdragon 865</td>
                <td>250-350</td>
                <td>45-55°C</td>
            </tr>
            <tr>
                <td>Exynos 2100</td>
                <td>200-300</td>
                <td>50-60°C</td>
            </tr>
            <tr>
                <td>MediaTek Dimensity</td>
                <td>150-250</td>
                <td>40-50°C</td>
            </tr>
        </table>
    </div>

    <div class="section">
        <h2 class="section-title">📞 Hỗ trợ</h2>
        <p>Gặp sự cố? Mở issue tại: <br>
        <a href="https://github.com/d4m-dev/Xmrig/issues">https://github.com/d4m-dev/Xmrig/issues</a></p>
    </div>

    <div class="section">
        <h2 class="section-title">📜 Giấy phép</h2>
        <p>Dự án được phân phối theo giấy phép MIT. Xem file <a href="LICENSE">LICENSE</a> để biết thêm chi tiết.</p>
    </div>

    <div class="footer">
        <p>🔗 <strong>Liên kết hữu ích:</strong></p>
        <a href="https://xmrig.com">XMRig Official</a> | 
        <a href="https://www.getmonero.org">Monero Official</a> | 
        <a href="https://termux.com">Termux Official</a>
    </div>
