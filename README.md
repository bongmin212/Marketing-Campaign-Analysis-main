# Bối cảnh Dự án
Chiến dịch tiếp thị liên quan đến phân tích này nhằm mục đích tối đa hóa lợi tức đầu tư (ROI) cho các chiến dịch quảng cáo của khách hàng. Vào năm 2019, hai chiến dịch quảng cáo riêng biệt đã được thực hiện trên Facebook và AdWords. 
Phân tích này được thực hiện để xác định nền tảng nào mang lại kết quả tốt hơn về các chỉ số hiệu suất chính, bao gồm số lượt nhấp vào quảng cáo, chuyển đổi và hiệu quả chi phí tổng thể. 
Bằng cách khám phá những thông tin chi tiết này, công ty có thể phân bổ ngân sách tốt hơn và tối ưu hóa các chiến lược tiếp thị trong tương lai cho khách hàng của mình.

# Cấu trúc Dữ liệu 
Tập dữ liệu chứa 365 bản ghi tương ứng với mỗi ngày trong năm 2019. Các đặc điểm chính bao gồm:
- **Date (Ngày):** Ngày thu thập dữ liệu.
- **Facebook Ad Campaign (Chiến dịch Quảng cáo Facebook):** Thông tin về số lượt nhấp, chuyển đổi và chi phí quảng cáo cho Facebook.
- **AdWords Ad Campaign (Chiến dịch Quảng cáo AdWords):** Dữ liệu tương tự cho nền tảng AdWords.

Các bảng chính trong tập dữ liệu:
- Facebook Ad Campaign (Chiến dịch Quảng cáo Facebook)
- AdWords Ad Campaign (Chiến dịch Quảng cáo AdWords)

Trước khi tiến hành phân tích, tập dữ liệu đã trải qua kiểm tra chất lượng để đảm bảo tính đầy đủ và nhất quán. 

# Tóm tắt Điều hành
## Tổng quan về Phát hiện
- **Quảng cáo Facebook vượt trội so với AdWords:** Số lượng chuyển đổi trung bình từ quảng cáo Facebook cao hơn đáng kể so với AdWords, với tỷ lệ chuyển đổi trung bình là 11,74 so với 5,98 của AdWords.
- **Tần suất Chuyển đổi:** Quảng cáo Facebook cho thấy các ngày có chuyển đổi cao thường xuyên hơn, trong khi AdWords trải qua tỷ lệ chuyển đổi thấp hoặc trung bình, với khoảng trống đáng chú ý về số lượng chuyển đổi.
- **Tương quan giữa Lượt nhấp và Doanh số:** Có một tương quan thuận mạnh mẽ (0,87) giữa lượt nhấp vào quảng cáo Facebook và doanh số, cho thấy rằng nhiều lượt nhấp vào quảng cáo Facebook trực tiếp mang lại nhiều doanh số hơn. Đối với AdWords, tương quan ở mức trung bình (0,45), cho thấy các yếu tố khác ảnh hưởng đến hiệu quả bán hàng của nó.
- **Hiệu quả Chi phí (Xu hướng CPC):** Chi phí quảng cáo biến động trong năm. Đáng chú ý, tháng 5 và tháng 11 cho thấy chi phí trên mỗi chuyển đổi thấp nhất, cho thấy đó là những giai đoạn tiết kiệm chi phí hơn, trong khi tháng 2 có CPC cao nhất, đảm bảo việc xem xét lại chiến lược quảng cáo trong tháng đó.
- **Kiểm định Giả thuyết:** Giả thuyết rằng quảng cáo Facebook tạo ra nhiều chuyển đổi hơn AdWords được phân tích thống kê hỗ trợ mạnh mẽ, với T-statistic là 32,88 và p-value là 9,35e-134.
- **Mô hình Dự đoán:** Mô hình hồi quy tuyến tính cho thấy khả năng dự đoán mạnh mẽ đối với chuyển đổi trên Facebook, với điểm R2 là 76,35%, giúp doanh nghiệp dự báo chuyển đổi trong tương lai dựa trên lượt nhấp quảng cáo.

## Thông tin chi tiết chính:
- **Quảng cáo Facebook Vô Cùng Hiệu Quả:** Với khả năng tương quan mạnh mẽ giữa lượt nhấp và chuyển đổi, doanh nghiệp nên xem xét tăng đầu tư vào quảng cáo Facebook để thúc đẩy bán hàng.
- **Cần Tối ưu hóa AdWords:** Dù AdWords đóng góp vào chuyển đổi, hiệu quả của nó hạn chế hơn. Khuyến nghị phân tích sâu hơn về chiến lược chiến dịch.
- **Phân bổ Ngân sách:** Để tối đa hóa ROI, phân bổ nhiều ngân sách hơn vào các tháng có CPC lịch sử thấp, như tháng 5 và tháng 11, và tối ưu hóa chiến dịch trong suốt những thời kỳ CPC cao, như tháng 2.
- **Tập trung Ngày trong tuần:** Nhấn mạnh ngân sách quảng cáo và mọi nỗ lực vào Thứ Hai và Thứ Ba, đều đặn cho thấy tỷ lệ chuyển đổi cao hơn.

# Phân tích Chuyên sâu
## Phân tích Nhấp chuột vào Quảng cáo:
Tất cả các biểu đồ liên quan đến nhấp chuột và chuyển đổi cho thấy sự phân bố tương đối đối xứng, chỉ ra sự phân bổ tương đối đồng đều của các chỉ số này.
![fb ad conversions](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/fb%20ad%20conversions.png)
![ad words ad conversions](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/adwords%20ad%20conversions.png)

## Tỷ lệ Chuyển đổi:
- **Facebook:** Quan sát thấy các ngày có chuyển đổi cao diễn ra thường xuyên hơn so với AdWords, nền tảng thường có xu hướng ở mức chuyển đổi thấp hoặc trung bình.
- **AdWords:** Không có chuyển đổi nào được quan sát thấy trong phạm vi 10-15, cho thấy cần phải xem xét lại các chiến lược.
![conversion rates](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/daily%20conversions%20by%20categories.png)

## Hiệu quả Chi phí:
Mối tương quan dương mạnh (0,87) giữa các lượt nhấp vào quảng cáo Facebook và doanh số bán hàng, cho thấy quảng cáo Facebook rất hiệu quả trong việc thúc đẩy doanh số.
Quảng cáo AdWords cũng tương quan tích cực với doanh số, nhưng với hệ số ở mức vừa phải (0,45), cho thấy các yếu tố khác ảnh hưởng đến hiệu quả của chúng.
![clicks_conversions](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/clicks_conv.png)

## Kiểm định Giả thuyết:
_Giả thuyết: Quảng cáo trên Facebook sẽ dẫn đến số lượng chuyển đổi lớn hơn so với AdWords._
- Tỷ lệ chuyển đổi trung bình của Facebook (11,74) cao hơn đáng kể so với AdWords (5,98).
- T-statistic: 32,88, p-value: 9,35e-134 — bằng chứng mạnh mẽ củng cố rằng Facebook tạo ra nhiều chuyển đổi hơn AdWords.

**Khuyến nghị:** Phân bổ lại nhiều nguồn lực hơn vào quảng cáo trên Facebook để tận dụng tối đa tỷ lệ chuyển đổi cao hơn.

## Mô hình Dự báo:
Mô hình hồi quy tuyến tính cho thấy nhấp chuột vào quảng cáo Facebook giải thích được 76,35% sự thay đổi trong các chuyển đổi. Khả năng dự báo này giúp ích trong việc lập kế hoạch và tối ưu hóa các chiến dịch trong tương lai.

![fb regression](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/fb%20regression.png)

## Xu hướng (Tỷ lệ Nhấp CTR và Tỷ lệ Chuyển đổi):
- **Hiệu suất Theo Ngày trong Tuần:** Chuyển đổi có tính chất nhất quán, nhưng Thứ Hai và Thứ Ba có tỷ lệ chuyển đổi cao hơn, thể hiện sự tương tác với người dùng ở đầu tuần tăng cao.
  
    ![fb weekday](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/fb%20weekly%20conversion.png)
- **Xu hướng Chuyển đổi Theo Tháng:** Sự biến động về tỷ lệ chuyển đổi được ghi nhận trong các tháng 2, 4, 5, 6, 8 và 11, có thể do xu hướng theo mùa hoặc thay đổi chiến lược tiếp thị.
  
    ![fb monthly](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/fb%20monthly%20conversion.png)
- **Xu hướng CPC:** Tháng 5 và tháng 11 có giá trị CPC thấp hơn, biểu thị đây là các giai đoạn hiệu quả quảng cáo cao hơn, trong khi tháng 2 chứng kiến CPC cao hơn.
  
    ![fb monthly cpc](https://github.com/bongmin212/Marketing-Campaign-Analysis/blob/main/images/fb%20monthly%20cpc.png)

# Các Khuyến nghị
Dựa vào những phát hiện từ phân tích này, chúng tôi đưa ra những khuyến nghị sau cho các chiến dịch quảng cáo trong tương lai:
1. **Phân bổ Lại Ngân sách cho Quảng cáo Facebook:** Ưu tiên các chiến dịch trên Facebook do có tỷ lệ chuyển đổi vượt trội, và thực hiện thử nghiệm A/B với các ý tưởng quảng cáo khác nhau để tối ưu hóa.
2. **Tối ưu hóa AdWords Đi Kèm Thử nghiệm A/B:** Rà soát và điều chỉnh chiến lược AdWords thông qua thử nghiệm A/B để khắc phục những hạn chế trong chuyển đổi và cải thiện hiệu suất.
3. **Sử dụng Căn cứ Dự báo:** Tận dụng dữ liệu từ mô hình hồi quy để đặt ra những mục tiêu thực tế và tối ưu hóa việc chi tiêu cho quảng cáo Facebook.
4. **Triển khai Các Chiến dịch Vào Thứ Hai và Thứ Ba:** Tập trung nỗ lực vào những ngày làm việc này khi mà mức độ tương tác của người dùng gắn với các chuyển đổi ở mức cao nhất.
5. **Điều chỉnh Ngân sách Dựa trên Xu hướng CPC:** Dịch chuyển chi tiêu sang các tháng có chi phí thấp hơn như tháng 5 và tháng 11 để phát huy tối đa hiệu quả chi phí.


_Vui lòng tặng 🌟 nếu bạn thấy kho lưu trữ này hữu ích theo bất kỳ cách nào._
