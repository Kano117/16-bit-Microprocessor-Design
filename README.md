# Thiết kế vi xử lý 16 bit theo kiến trúc tập lệnh đơn giản

## Project

Thiết kế vi xử lý 16 bit theo kiến trúc tập lệnh đơn giản  
• Vi xử lý / bộ xử lý: xử lý dữ liệu, kiểm soát hệ thống, I/O, bộ nhớ, thực hiện hầu hết các tác vụ tính toán, xử lý dữ liệu  
• Datapath: thực hiện chính nhiệm vụ tính toán, xử lý dữ liệu bao gồm các bộ xử lý, các thành phần nhớ, các thành phần liên kết I/O, khác  
• Controller: tạo tín hiệu điều khiển các khối trong datapath  
• 16 bit: Data Bus 16 bit -> 1 đơn vị dữ liệu xử lý 16 bit -> ngăn thanh ghi 16 bit -> ngăn bộ nhớ 16 bit  
• Tập lệnh đơn giản: tập lệnh tuỳ biến định dạng độ dài 16 bit  
• Cân đối giữa tính hiệu quả và kích cỡ của chương trình với chi phí và hiệu suất của bộ xử lý  
• Tối ưu thiết kế theo hiệu năng, định thời, tài nguyên, công suất

## Tập lệnh

• Tập lệnh 16 bit phân loại theo cấu trúc:  
• RRR  
• RRI  
• RI  
• Thanh ghi: 8 thanh ghi 16 bit, được đánh địa chỉ trực tiếp (0 -> 7)  
• Bộ nhớ chương trình 16 bit, địa chỉ từ 6 bit trở lên (64x16b)  
• Bộ nhớ dữ liệu 16 bit, địa chỉ từ 5 bit trở lên (32x16b), ít nhất 2 địa chỉ sử dụng cho I/O (16 bit input, 16 bit output)

## Quy trình thiết kế

• Phát triển, mở rộng tập lệnh  
• Phân loại tập lệnh  
• Xây dựng một số phần mềm thử nghiệm hoạt động của CPU (ASM)  
• Biên dịch ASM, nạp và kiểm tra hoạt động của CPU  
• Kiểm tra hiệu năng hoạt động của CPU  
• Kiểm tra định thời mức cổng  
• Kiểm tra tài nguyên và công suất  
• Tối ưu hiệu năng hoạt động của CPU  
• Tối ưu định thời mức cổng  
• Tối ưu tài nguyên và công suất  
• Xây dựng lưu đồ tập lệnh  
• Xây dựng sơ đồ ASM  
• Xác định các thành phần cần có trong datapath  
• Thiết kế datapath -> xác định các tín hiệu điều khiển cần  
• Thiết kế controller  
• Hoàn chỉnh thiết kế CPU
