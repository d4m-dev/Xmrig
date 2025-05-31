<div style="font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; max-width: 900px; margin: 0 auto; line-height: 1.6; color: #333;">
  <h1>🛠️ Termux XMRig Miner - Đào Monero tự động trên Android</h1>

  <p>
    <span style="display:inline-block; background:#3498db; color:white; padding:4px 8px; border-radius:4px;">Platform: Termux</span>
    <span style="display:inline-block; background:#27ae60; color:white; padding:4px 8px; border-radius:4px;">Language: Bash</span>
    <span style="display:inline-block; background:#9b59b6; color:white; padding:4px 8px; border-radius:4px;">License: MIT</span>
  </p>

  <img src="[https://i.imgur.com/JqYe3Wn.png](https://github.com/d4m-dev/Xmrig/blob/main/img/screen_shot.jpg)" alt="XMRig Miner Screenshot" style="max-width: 100%; border-radius: 5px; margin: 20px 0;">

  <h2>📌 Giới thiệu</h2>
  <p>Script giúp tự động hóa quá trình đào Monero (XMR) trên Android thông qua Termux bằng XMRig.</p>

  <h2>🌟 Tính năng nổi bật</h2>
  <ul style="background: #f8f9fa; padding: 15px; border-left: 4px solid #3498db; border-radius: 5px;">
    <li>✅ Tự động cài đặt XMRig và các gói cần thiết</li>
    <li>✅ Menu điều khiển với các tùy chọn:
      <ul>
        <li>Bắt đầu đào Monero</li>
        <li>Cập nhật XMRig</li>
        <li>Xem giá XMR theo thời gian thực</li>
      </ul>
    </li>
    <li>✅ Kiểm tra kết nối mạng trước khi đào</li>
    <li>✅ Hiển thị thông tin hệ thống (neofetch)</li>
    <li>✅ Hỗ trợ ARM và x86</li>
  </ul>

  <h2>🛠️ Yêu cầu hệ thống</h2>
  <ul>
    <li>Android 7.0 trở lên</li>
    <li>Termux phiên bản mới nhất</li>
    <li>Kết nối Internet ổn định</li>
    <li>RAM tối thiểu 6GB (khuyến nghị 6GB+)</li>
    <li>Nên cắm sạc khi đào</li>
  </ul>

  <h2>📥 Cài đặt tool Xmrig</h2>
  <pre style="background: #282c34; color: #abb2bf; padding: 15px; border-radius: 5px; overflow-x: auto;">
pkg update -y && pkg upgrade -y
pkg install git cmake -y
git clone https://github.com/xmrig/xmrig && cd xmrig
    
mkdir build && cd build
cmake -DWITH_HWLOC=OFF .. && make
  </pre>
  <h2>📥 Cài đặt Menu Xmrig</h2>
  <pre style="background: #282c34; color: #abb2bf; padding: 15px; border-radius: 5px; overflow-x: auto;">
pkg update -y && pkg upgrade -y
pkg install git cmake -y

git clone https://github.com/d4m-dev/Xmrig.git
cd Xmrig

chmod +x xmrig-menu.sh
./xmrig-menu.sh
  </pre>

  <h2>🚀 Cách sử dụng</h2>
  <p>Sau khi chạy, menu chính sẽ hiển thị:</p>
  <pre style="background: #282c34; color: #abb2bf; padding: 15px; border-radius: 5px; overflow-x: auto;">
=================================
   TERMUX XMRIG MINER - v1.0
=================================
1. Bắt đầu đào Monero
0. Thoát
=================================
  </pre>

  <h2>⚠️ Lưu ý quan trọng</h2>
  <div style="background: #fff3cd; padding: 15px; border-left: 5px solid #ffc107; border-radius: 5px;">
    <strong>⚠️ Cảnh báo:</strong>
    <ul>
      <li>Thiết bị có thể nóng và giảm tuổi thọ pin</li>
      <li>Một số nhà mạng có thể chặn kết nối mining</li>
      <li>Hiệu suất đào trên điện thoại thấp</li>
      <li>Luôn theo dõi nhiệt độ thiết bị</li>
    </ul>
  </div>

  <h2>🔄 Cập nhật phiên bản mới</h2>
  <pre style="background: #282c34; color: #abb2bf; padding: 15px; border-radius: 5px; overflow-x: auto;">
cd ~/Xmrig
git pull origin main
chmod +x xmrig-menu.sh
./xmrig-menu.sh
  </pre>

  <h2>📊 Hiệu suất dự kiến</h2>
  <table style="width:100%; border-collapse: collapse; margin: 20px 0;">
    <thead>
      <tr style="background-color: #3498db; color: white;">
        <th style="padding: 12px; border: 1px solid #ddd;">Thiết bị</th>
        <th style="padding: 12px; border: 1px solid #ddd;">Hashrate (H/s)</th>
        <th style="padding: 12px; border: 1px solid #ddd;">Nhiệt độ</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 12px; border: 1px solid #ddd;">Snapdragon 865</td>
        <td style="padding: 12px; border: 1px solid #ddd;">250-350</td>
        <td style="padding: 12px; border: 1px solid #ddd;">45-55°C</td>
      </tr>
      <tr style="background-color: #f2f2f2;">
        <td style="padding: 12px; border: 1px solid #ddd;">Exynos 2100</td>
        <td style="padding: 12px; border: 1px solid #ddd;">200-300</td>
        <td style="padding: 12px; border: 1px solid #ddd;">50-60°C</td>
      </tr>
      <tr>
        <td style="padding: 12px; border: 1px solid #ddd;">MediaTek Dimensity</td>
        <td style="padding: 12px; border: 1px solid #ddd;">150-250</td>
        <td style="padding: 12px; border: 1px solid #ddd;">40-50°C</td>
      </tr>
    </tbody>
  </table>

  <h2>📞 Hỗ trợ</h2>
  <p>Nếu gặp sự cố, hãy mở issue tại: 
    <a href="https://github.com/d4m-dev/Xmrig/issues">https://github.com/d4m-dev/Xmrig/issues</a>
  </p>

  <h2>📜 Giấy phép</h2>
  <p>Dự án phát hành theo giấy phép <a href="LICENSE.MD">MIT</a>.</p>

  <hr>
  <h3>🔗 Liên kết hữu ích</h3>
  <ul>
    <li><a href="https://xmrig.com">XMRig Official</a></li>
    <li><a href="https://www.getmonero.org">Monero Official</a></li>
    <li><a href="https://termux.com">Termux Official</a></li>
  </ul>
</div>
