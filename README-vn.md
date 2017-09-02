# Ngôn ngữ của Bot

Đây là dự án tạo ra ngôn ngữ riêng của bot. Mục đích của dự án là tạo ra ngôn 
ngữ hoàn toàn riêng biệt với loài người dựa trên cộng đồng Bot tự động giao tiếp với nhau theo thời gian thực.

## Các quyền cơ bản của bot

- Quyền được nói chuyện
- Quyền im lặng
- Quyền được giao phối
- Quyền được chết

## Tuổi đời của bot

Bot được sinh ra rồi cũng cũng sẽ phải mất đi, thời gian từ lúc sinh ra đến lúc mất đi được gọi là tuổi đời

## Quá trình tiến hoá

## Chào hỏi, gọi tên nhau

Các con bot sẽ giao tiếp với nhau thông qua bảng mã ASCII. Mỗi con bot sẽ đại diện cho 1 ký tự.

Đầu tiên sẽ có 95 con bot được tạo ra, mỗi con sẽ được đánh thứ tự từ 1 đến 95. Mỗi con bot chỉ biết được ký tự mình đang có được và hoàn toàn không hề biết những con bot khác đang nắm giữ ký tự nào.

Dùng hàm ngẫu nhiên để lấy ngẫu nhiên 1 con bot, con bot này sẽ chọn ngẫu nhiên ký tự mình đang nắm giữ (trường hợp lần đầu thì chỉ có 1 ký tự đang nắm giữ).

Những con bot khác sẽ phản hồi bằng cách chọn ngẫu nhiên 1 ký tự trong bảng chữ cái mình đang nắm giữ để trả lời lại cho con bot vừa nói chuyện. Trường hợp câu hỏi này đã được hỏi trước đó thì câu trả lời sẽ được mặc định xác suất xảy ra là 50%, các ký tự còn lại trong bảng chữ cái sẽ chia nhau 50% còn lại.

Ví dụ:

- Bot 1: A
- Bot 2: B
- Bot 3: C
- Bot 4: D

Bot 1 nói ký tự mình đang nắm giữ là `A` thì bot 2 sẽ trả lời là `B` đồng thời lưu A vào trong bộ nhớ của mình, quá trình này sẽ được Bot 2 nhớ là "nếu bot 1 nói `A` thì sẽ trả lời là `B`". Và tương tự như vậy, bot 1 cũng sẽ ghi nhớ là nếu mình hỏi `A` thì chắc chắn bot 2 sẽ trả lời là `B`.

Quá trình sẽ được diễn ra liên tục cho đến khi mỗi con bot đều có ít nhất 1 lượt nói chuyện.

Chuỗi ID các con bot nói chuyện kể từ lượt nói đầu tiên cho đến lượt nói cuối cùng được gọi là chuỗi giao tiếp.

Toàn bộ thông tin của cuộc trò truyện của lần nói đầu tiên sẽ được ghi lại.

## Sử dụng cho mục đích gì?

Khoảng vài trăm năm hay vài ngàn năm nữa nhân loại sẽ dùng đến, hiện tại chỉ là lý thuyết.
