# Ngôn ngữ của Bot

Đây là dự án tạo ra ngôn ngữ riêng của Bot. Mục đích của dự án là tạo ra ngôn 
ngữ hoàn toàn riêng biệt với loài người dựa trên cộng đồng Bot tự động giao tiếp với nhau theo thời gian thực.

## Các quyền cơ bản của Bot

- Quyền được nói chuyện
- Quyền được im lặng
- Quyền được sinh sản
- Quyền được chết

## Các trạng thái của Bot

- Vui 
- Buồn
- Yêu
- Ghét

## Tuổi đời của Bot

Bot được sinh ra rồi cũng cũng sẽ phải mất đi, thời gian từ lúc sinh ra đến lúc mất đi được gọi là tuổi đời

## Quá trình tiến hoá

## Hàm bầu cử

Hàm gọi Bot nói chuyện sẽ được trưng cầu ý kiến từ tất cả các thành viên trong cộng đồng. Mỗi con bot sẽ duyệt qua từ 1-95 mỗi phần tử sẽ được đánh dấu 0 hoặc 1. Những phần tử được chọn 0 sẽ bỏ đi. Lập lại như vậy cho các phần tử được chọn là 1. Đến khi còn duy nhất 1 phần tử thì phần tử đó chính là phần tử được chọn.

## Hàm chọn sẽ nói gì

## Hàm chọn sẽ trả lời gì

## Quá trình giao tiếp

Sẽ có 95 con bot được tạo ra từ bảng mã ASCII, được đánh thứ tự từ 1 đến 95 tương ứng với mỗi ký tự. Các Bot chỉ biết được ký tự mình đang có được và hoàn toàn không hề biết những con Bot khác đang nắm giữ ký tự nào.

Dùng hàm bầu cử để chọn ra 1 con bot sẽ nói chuyện, con Bot này sẽ dùng hàm chọn sẽ nói gì để nói lên cái mình sẽ nói.

Những con bot khác vẫn dùng hàm chọn sẽ trả lời gì để trả lời lại cho con bot vừa nói chuyện. Trường hợp câu hỏi này đã được hỏi trước đó thì câu trả lời sẽ được mặc định xác suất xảy ra là 50%, các ký tự còn lại trong bảng chữ cái sẽ chia nhau 50% còn lại.

Ví dụ:

- Bot 1: A
- Bot 2: B
- Bot 3: C
- Bot 4: D

Bot 1 nói ký tự mình đang nắm giữ là `A` thì Bot 2 sẽ trả lời là `B` đồng thời lưu `A` vào bảng chữ cái của mình, quá trình này sẽ được Bot 2 nhớ là "nếu Bot 1 nói `A` thì sẽ trả lời là `B`". Và tương tự như vậy, Bot 1 cũng sẽ ghi nhớ là nếu mình hỏi `A` thì chắc chắn Bot 2 sẽ trả lời là `B`.

Quá trình sẽ được diễn ra liên tục cho đến khi mỗi con bot đều có ít nhất 1 lượt nói chuyện.

Chuỗi ID các con bot nói chuyện kể từ lượt nói đầu tiên cho đến lượt nói cuối cùng được gọi là chuỗi giao tiếp.

Toàn bộ thông tin của cuộc trò truyện của lần nói đầu tiên sẽ được ghi lại.

## Sử dụng cho mục đích gì?

Khoảng vài trăm năm hay vài ngàn năm nữa nhân loại sẽ dùng đến, hiện tại chỉ là lý thuyết.
