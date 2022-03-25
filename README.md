## IN BIỂU DIỄN NHỊ PHÂN CỦA SỐ NGUYÊN
### Input : số nguyên n
### Output : chuỗi các số nhị phân
### Describe :
    + Trường hợp suy biến : Khi n chia nguyên cho 2 bằng 0 thì trả lại n chia dư 2
    + Trường hợp chung : Sử dụng lời gọi đệ quy với tham số n chia nguyên cho 2 rồi ghép với xâu n chia dư 2

## PHÂN TÍCH SỐ NGUYÊN THÀNH TÍCH CÁC THỪA SỐ NGUYÊN TỐ
### Input : số nguyên n, mảng các số nguyên tố nhỏ hơn hoặc bằng n (primes), vị trí duyệt mảng các số nguyên tố (index)
### Output : chuỗi các thừa số nguyên tố
###  Describe :
    + Trường hợp suy biến : Khi index >= độ dài primes và n <= 1
    + Trường hợp chung : 
        + Nếu n chia hết cho primes[index], trả lại chuỗi primes[index] ghép với lời gọi đệ quy với tham số n chia nguyên cho primes[index], primes và index=0 (duyệt lại từ đầu mảng primes)
        + Ngược lại trả về lời gọi đệ quy với tham số n, primes, index+1

## TÌM SỐ FIBONACCI THỨ N
### Input : n
### Output : số fibonacci thứ n
### Describe :
    + Trường hợp suy biến : Nếu n < 3 và n > 0, trả lại 1
    + Trường hợp chung : Trả lại lời gọi đệ quy với tham số n-1 cộng với lời gọi đệ quy với tham số n-2 

## BÀI TOÁN THÁP HÀ NỘI
### Input : số đĩa n, a:cột ban đầu, b:cột đích, c:cột trung gian
### Output : In ra màn hình các lần di chuyển đĩa
### Describe :
    + Trường hợp suy biến : Khi n = 1, di chuyển trực tiếp từ a sang b
    + Trường hợp chung :
        + Lời gọi đệ quy di chuyển n-1 đĩa từ a sang c thông qua b
        + Di chuyển 1 đĩa từ a sang b
        + Lời gọi đệ quy di chuyển n-1 đĩa từ c sang b thông qua a  
