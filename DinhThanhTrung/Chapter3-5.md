#Câu 5: Tìm ra lỗi trong ca kiểm thử theo phương thức JUnit và mô tả theo mô hình RIPR
-Reachability (khả năng tiếp cận): Lỗi trong ca kiểm thử nằm ở phương thức so sánh chuỗi equals().
-Infection (Sự nhiễm lỗi): Hàm kiểm thử sẽ nhiễm lỗi khi chuỗi trong mảng name và chuỗi dùng để so sánh có phân biệt chữ hoa ("alex" và "Alex"). Hàm equals() sẽ trả về kết quả false.
-Propagation (Sự lan truyền): Hàm assertTrue sẽ không trả về chuỗi "Sort method".
-Revealabilty (Sự quan sát được): Người kiểm thử sẽ thấy kết quả trả về không như dự tính (chương trình trả về chuỗi "Sort method")
Ở đây nên sử dụng hàm equalsIgnoreCase().