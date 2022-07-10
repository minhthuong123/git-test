# git-test
Các thành phần React
Một component trả về một tập hợp các phần tử React
sẽ xuất hiện trên màn hình
###Các thành phần cho phép bạn chia giao diện người dùng của mình thành
các mảnh độc lập, có thể tái sử dụng
###Các thành phần cũng chấp nhận đầu vào
###Các loại thành phần khác nhau có thể được định nghĩa trong React

Tên thành phần do người dùng xác định phải luôn
bắt đầu bằng chữ in hoa
- Chúng biên dịch thành React.createElement (. . .)
### Thẻ bắt đầu bằng chữ thường được coi là
Thẻ DOM
– Các thành phần tích hợp

## Tiểu bang
Mỗi thành phần có thể lưu trữ cục bộ của riêng mình
thông tin trong "trạng thái" của nó
– Riêng tư và được kiểm soát hoàn toàn bởi các thành phần
– Có thể được thông qua làm đạo cụ cho trẻ em
### Chỉ các thành phần lớp mới có thể có tiểu bang địa phương

## Tiểu bang
###Tiểu bang được tuyên bố trong
Constructor:
class Menu mở rộng Component {
constructor(đạo cụ) {
siêu (đạo cụ);
this.state = {
selectedDish: null
}
}
. . .
}
### Trạng thái chỉ nên được sửa đổi
sử dụng setState()
onDishSelect(món ăn) {
this.setState({
selectedDish: món ăn
});
}
### Không bao giờ làm như sau:
this.state.selectedDish = món ăn;
