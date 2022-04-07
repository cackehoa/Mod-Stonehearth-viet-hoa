# Mod Stonehearth việt hóa
Mod Stonehearth ngôn ngữ tiếng Việt
# Lời nói đầu:
Mình chỉ mới bắt đầu dự án dịch Stonehearth nên mọi thứ phải từ từ cập nhật khi mình có thời gian. Mong mọi người ủng hộ.

Nếu có vấn đề gì về dịch thuật các bạn có thể theo liên hệ với mình để hoàn thiện bản mod này hơn.
# Giới thiệu về game
Trong Stonehearth, bạn đi tiên phong trong một thế giới sống đầy ấm áp, anh hùng và bí ẩn. Giúp một nhóm nhỏ người định cư xây dựng một ngôi nhà cho chính họ ở một vùng đất bị lãng quên. Bạn sẽ cần thiết lập nguồn cung cấp thực phẩm, xây dựng nơi trú ẩn, bảo vệ người dân của bạn, theo dõi tâm trạng của họ và tìm cách phát triển và mở rộng, đối mặt với thách thức ở mọi bước.

Bắt đầu từ địa hình được tạo theo thủ tục với các cuộc gặp gỡ AI động, Stonehearth kết hợp quản lý cộng đồng và chiến đấu với khả năng xây dựng vô hạn. Nó được thiết kế để có thể sửa đổi ở mọi cấp độ, từ thành phố của bạn đến những người và sinh vật sống trên thế giới, đồng thời sẽ gửi kèm theo các công cụ và tài liệu để bạn thêm các tùy chỉnh của riêng mình vào trò chơi và chia sẻ chúng với bạn bè.
# Hướng dẫn
## Cài đặt trò chơi

Cài đặt trò chơi Stonehearth và chạy thử trước khi cài mod việt hóa

Đề nghị mua trò chơi để ủng hộ nhà sản xuất.

## Phiên bản yêu cầu: v1.1.0.rel.949

Mình dịch trên phiên bản v1.1.0.rel.949 nên có thể không chạy hoặc có lỗi trên phiên bản khác

## Cài đặt việt hóa

- Tải tất cả thư mục [startermod_locale](startermod_locale/) trong này
- Copy và dán vào thư mục **Stonehearth.v1.1.0.rel.949\mods**
- Khởi động game vào **Mod** -> chọn **Mod tiếng Việt**
- **Settings** -> **System** -> **Mod** -> **Language** -> chọn **Tiếng Việt**
# Cách hoạt động
## Tệp kê khai manifest.json sử dụng dòng: <br>
````
"mixintos" : {
      "stonehearth/locales/supported_languages.json" : "file(added_languages.json)"
   }
````
Điều này khiến tất cả dữ liệu trong added_languages.json được thêm vào danh sách các ngôn ngữ được hỗ trợ được nhận dạng bởi stonehearth mod.
## Chỉ định ngôn ngữ Vietnamese trong added_languages.json:
````
"vi": {
         "display_name": "Vietnamese"
      }
````
## Thêm các bản dịch của cơ bản và các mod khác:
````
"overrides": {
    "candledark/locales/vi.json": "file(translations/candledark/vi.json)",
    "debugtools/locales/vi.json": "file(translations/debugtools/vi.json)",
    "northern_alliance/locales/vi.json": "file(translations/northern_alliance/vi.json)",
    "stonehearth/locales/vi.json": "file(translations/stonehearth/vi.json)",
    "rayyas_children/locales/vi.json": "file(translations/rayyas_children/vi.json)",
    "frostfeast/locales/vi.json": "file(translations/frostfeast/vi.json)"
   }
````
Ghi đè này hiểu quả như bạn thêm các tệp tin ngôn ngữ tương ứng từng mod
## Cách dịch:
- Bạn có thể dễ dàng dịch các tập tin vi.json trong các thư mục tương ứng
- Không sửa đổi nội dung bên trái dấu ':'
- Không sửa đổi nội dung bên trong dấu ngoặc vuông '[' hoặc ']'
- Example:
  ````
  "ai": {
   "actions": {
      "status_text": {
         "chase_entity": "chasing [name(data.target)]",
  ````
- Chuỗi cần dịch là "chasing [name(data.target)]"
- Lưu ý, KHÔNG dịch phần "[name (data.target)]". Đây là chuỗi đặc biệt. Tên của mục tiêu sẽ thay thế "[name (data.target)]" trong trò chơi.
- Không thay thế "[name (data.target)]" bằng các chuỗi đặc biệt khác là tốt nhất.
- Bạn có thể di chuyển "[name (data.target)]" đến các vị trí khác nhau trong chuỗi.
- Bạn có thể dịch nó như thế này bằng tiếng Việt
````
  "ai": {
   "actions": {
      "status_text": {
         "chase_entity": "Đuổi theo [name(data.target)]",
````
- Hoặc tiếng Nhật (Lấy ví dụ cách đổi chỗ chuỗi đặt biệt để sau này cần)
````
  "ai": {
   "actions": {
      "status_text": {
         "chase_entity": "[name(data.target)]を追う",
````
# Xem thêm hướng dẫn sử dụng github

Nếu chưa biết cách sữ dụng [github](https://github.com) thì bạn có thể xem thêm [ở đây](/huongdan/HUONG-DAN.md)

# Liên lạc và ủng hộ
Ủng hộ tại: [Playerduo](https://playerduo.com/cackehoa)

Fanpage: [fb](https://www.facebook.com/cackehoa)

Discord: [Discord](https://discord.gg/Z5C98FG)

Youtube: [Cắc kè hoa](https://www.youtube.com/c/Cắckèhoa)
