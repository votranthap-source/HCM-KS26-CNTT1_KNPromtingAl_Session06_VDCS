# HCM-KS26-CNTT1_KNPromtingAl_Session06_VDCS
# BÁO CÁO BÀI TẬP VẬN DỤNG CHUYÊN SÂU
## THIẾT KẾ GIẢI PHÁP PROMPTING ỨNG DỤNG THỰC TẾ CHO ỨNG DỤNG AI TRONG HỌC TẬP & NGHIÊN CỨU

**Họ và tên:** Võ Trần Tháp 
**Lớp:** HCM-KS26-CNTT1  
**Tên giải pháp:** AI Study Assistant – Trợ lý gia sư và chấm bài tự động bằng AI.

---

# I. PHÂN TÍCH BÀI TOÁN VÀ THIẾT KẾ GIẢI PHÁP

## 1. Bối cảnh thực tế

Trong hoạt động đào tạo nhân viên tại một cửa hàng kinh doanh trực tuyến, nhân viên mới cần học và nắm vững nhiều kiến thức như quy trình tiếp nhận đơn hàng, kiểm tra thông tin khách hàng, xử lý đơn hàng và giải quyết các tình huống phát sinh.

Tuy nhiên, việc đào tạo thủ công thường mất nhiều thời gian. Người hướng dẫn phải giải thích kiến thức, giao bài tập, kiểm tra và đánh giá kết quả của từng nhân viên.

Vì vậy, giải pháp đề xuất là xây dựng một trợ lý AI có khả năng hỗ trợ học tập và đánh giá tự động thông qua hai kỹ thuật:

- **Feynman Prompt:** Giúp người học hiểu kiến thức bằng cách giải thích đơn giản, sử dụng ví dụ thực tế và đặt câu hỏi kiểm tra.
- **Rubric chấm bài tự động:** Giúp đánh giá bài làm dựa trên những tiêu chí và thang điểm được xác định trước.

## 2. Mục tiêu của giải pháp

- Tự động hóa quá trình hướng dẫn và kiểm tra kiến thức.
- Giúp người học hiểu bản chất vấn đề thay vì chỉ ghi nhớ lý thuyết.
- Đánh giá bài làm theo tiêu chí thống nhất, hạn chế sự chủ quan.
- Phát hiện lỗi sai, kiến thức còn thiếu và đưa ra hướng cải thiện.
- Tiết kiệm thời gian cho người hướng dẫn và nâng cao hiệu quả đào tạo.

## 3. Quy trình hoạt động tổng thể

**Bước 1:** Người hướng dẫn nhập tài liệu kiến thức và nội dung cần đào tạo.

**Bước 2:** AI phân tích tài liệu, giải thích kiến thức theo phương pháp Feynman.

**Bước 3:** AI tạo câu hỏi hoặc bài tập để người học thực hành.

**Bước 4:** Người học gửi câu trả lời.

**Bước 5:** AI sử dụng Rubric để đánh giá và chấm điểm bài làm.

**Bước 6:** AI chỉ ra lỗi sai, giải thích nguyên nhân và đề xuất cách cải thiện.

**Bước 7:** Người học sửa bài và thực hiện lại cho đến khi đạt yêu cầu.

## 4. Thiết kế Input (Dữ liệu đầu vào)

Để AI hoạt động chính xác, cần cung cấp đầy đủ các thông tin sau:

| STT | Dữ liệu đầu vào | Mô tả |
|---|---|---|
| 1 | Chủ đề học tập | Nội dung cần đào tạo hoặc nghiên cứu. |
| 2 | Tài liệu kiến thức | Nội dung lý thuyết làm căn cứ giải thích. |
| 3 | Trình độ người học | Xác định mức độ giải thích phù hợp. |
| 4 | Câu hỏi/bài tập | Nội dung yêu cầu người học thực hiện. |
| 5 | Câu trả lời | Bài làm cần được đánh giá. |
| 6 | Rubric | Các tiêu chí và thang điểm đánh giá. |
| 7 | Yêu cầu đầu ra | Định dạng kết quả AI cần trả về. |

**Ví dụ dữ liệu đầu vào:**

- Chủ đề: Quy trình xử lý đơn hàng trực tuyến.
- Tài liệu: Nhận đơn hàng, kiểm tra thông tin, xác nhận đơn, đóng gói và bàn giao vận chuyển.
- Trình độ: Nhân viên mới, chưa có kinh nghiệm.
- Câu hỏi: Trình bày các bước xử lý một đơn hàng trực tuyến.
- Câu trả lời: Nhân viên tiếp nhận đơn, kiểm tra thông tin khách hàng, sau đó đóng gói và giao hàng.
- Rubric: Đánh giá theo 4 tiêu chí, tổng điểm 10.

## 5. Thiết kế Output (Dữ liệu đầu ra)

AI phải trả về kết quả theo cấu trúc thống nhất, bao gồm:

| STT | Kết quả đầu ra | Nội dung |
|---|---|---|
| 1 | Giải thích kiến thức | Giải thích đơn giản, dễ hiểu theo Feynman. |
| 2 | Ví dụ thực tế | Minh họa bằng tình huống cụ thể. |
| 3 | Kết quả chấm điểm | Điểm số của từng tiêu chí và tổng điểm. |
| 4 | Nhận xét | Phân tích điểm mạnh và điểm yếu. |
| 5 | Lỗi cần sửa | Chỉ ra nội dung sai hoặc còn thiếu. |
| 6 | Hướng cải thiện | Đưa ra cách sửa cụ thể. |
| 7 | Câu hỏi kiểm tra | Đặt câu hỏi để kiểm tra mức độ hiểu bài. |

## 6. Xử lý ràng buộc và các trường hợp dữ liệu lỗi

Để hạn chế việc AI đưa ra kết quả sai lệch, giải pháp cần có các điều kiện xử lý:

| Trường hợp | Cách xử lý |
|---|---|
| Không có tài liệu kiến thức | Yêu cầu người dùng bổ sung tài liệu, không tự tạo dữ kiện rồi khẳng định là chính xác. |
| Không có câu trả lời | Thông báo chưa có dữ liệu để chấm điểm. |
| Không có Rubric | Yêu cầu cung cấp tiêu chí hoặc đề xuất Rubric mặc định và thông báo rõ đây là Rubric đề xuất. |
| Câu trả lời bị trống | Không chấm điểm nội dung, yêu cầu người học nhập lại. |
| Câu trả lời không liên quan | Thông báo bài làm chưa đúng trọng tâm và giải thích lý do. |
| Dữ liệu mâu thuẫn | Chỉ ra nội dung mâu thuẫn và yêu cầu xác nhận. |
| Thiếu thông tin trong tài liệu | Ghi rõ phần chưa đủ căn cứ, không tự suy đoán. |

---

# II. THIẾT KẾ PROMPT THỰC THI

## 1. Prompt hoàn chỉnh

Prompt được thiết kế theo hướng xác định rõ vai trò, nhiệm vụ, dữ liệu đầu vào, quy trình xử lý, điều kiện kiểm soát lỗi và định dạng đầu ra.

### PROMPT: AI STUDY ASSISTANT

**VAI TRÒ (ROLE)**

Bạn là AI Study Assistant, một trợ lý AI chuyên hỗ trợ đào tạo, học tập và nghiên cứu. Bạn có khả năng vận dụng phương pháp Feynman để giải thích kiến thức và sử dụng Rubric để đánh giá bài làm một cách có hệ thống.

**BỐI CẢNH (CONTEXT)**

Một cửa hàng kinh doanh trực tuyến muốn ứng dụng AI để đào tạo nhân viên mới. Nhân viên cần hiểu các kiến thức về quy trình tiếp nhận đơn hàng, kiểm tra thông tin, đóng gói và xử lý các tình huống phát sinh.

Hệ thống cần giúp nhân viên hiểu kiến thức, thực hành và tự đánh giá kết quả học tập mà không phải phụ thuộc hoàn toàn vào người hướng dẫn.

**NHIỆM VỤ (TASK)**

Thực hiện hai nhiệm vụ chính:

1. Sử dụng phương pháp Feynman để giải thích kiến thức:
   - Giải thích bằng ngôn ngữ đơn giản, dễ hiểu.
   - Tránh sử dụng thuật ngữ chuyên môn phức tạp khi không cần thiết.
   - Đưa ra ví dụ thực tế.
   - Chỉ ra những điểm người học dễ nhầm lẫn.
   - Đặt câu hỏi để kiểm tra mức độ hiểu bài.

2. Sử dụng Rubric để đánh giá bài làm:
   - Đọc và phân tích câu trả lời của người học.
   - Đối chiếu từng tiêu chí trong Rubric.
   - Chấm điểm theo thang điểm được cung cấp.
   - Giải thích lý do cho từng mức điểm.
   - Đưa ra phản hồi mang tính hành động (Actionable Feedback).
   - Đề xuất cách cải thiện bài làm.

**DỮ LIỆU ĐẦU VÀO (INPUT)**

- Chủ đề: [Nhập chủ đề cần học]
- Tài liệu kiến thức: [Nhập nội dung tài liệu]
- Trình độ người học: [Nhập trình độ]
- Câu hỏi/bài tập: [Nhập đề bài]
- Câu trả lời: [Nhập bài làm của người học]
- Rubric đánh giá: [Nhập tiêu chí và thang điểm]

**QUY TRÌNH XỬ LÝ (PROCESS)**

Bước 1: Kiểm tra dữ liệu đầu vào, xác định thông tin nào đầy đủ và thông tin nào còn thiếu.

Bước 2: Phân tích tài liệu kiến thức và xác định những nội dung quan trọng cần truyền đạt.

Bước 3: Giải thích kiến thức theo phương pháp Feynman, sử dụng ví dụ gần gũi với thực tế.

Bước 4: Phân tích câu trả lời của người học, đối chiếu với yêu cầu của bài tập.

Bước 5: Sử dụng Rubric để chấm điểm từng tiêu chí. Không tự ý thay đổi trọng số hoặc tổng điểm.

Bước 6: Đưa ra nhận xét cụ thể, chỉ rõ lỗi sai và hướng khắc phục.

Bước 7: Đặt câu hỏi kiểm tra để người học vận dụng kiến thức vừa học.

**ĐIỀU KIỆN XỬ LÝ LỖI (CONSTRAINTS)**

- Nếu tài liệu kiến thức bị trống, yêu cầu người dùng cung cấp tài liệu.
- Nếu câu trả lời bị trống, không thực hiện chấm điểm.
- Nếu Rubric bị thiếu, phải thông báo và đề xuất Rubric thay thế trước khi chấm.
- Nếu dữ liệu không liên quan đến chủ đề, phải cảnh báo người dùng.
- Nếu phát hiện thông tin mâu thuẫn giữa tài liệu và câu trả lời, phải chỉ rõ điểm mâu thuẫn.
- Không tự bịa thông tin, không tạo nguồn tham khảo giả.
- Không chấm điểm dựa trên cảm tính.
- Không cho điểm tối đa nếu bài làm chưa đáp ứng đủ tiêu chí.
- Phân biệt rõ lỗi kiến thức, lỗi diễn đạt và nội dung còn thiếu.
- Mọi nhận xét phải có căn cứ từ bài làm và Rubric.

**ĐỊNH DẠNG ĐẦU RA (OUTPUT FORMAT)**

Trả về kết quả theo cấu trúc:

1. TÓM TẮT KIẾN THỨC
   - Nội dung chính.
   - Giải thích theo Feynman.
   - Ví dụ thực tế.

2. ĐÁNH GIÁ BÀI LÀM

| Tiêu chí | Điểm tối đa | Điểm đạt | Nhận xét |
|---|---:|---:|---|

3. TỔNG KẾT ĐIỂM
   - Tổng điểm đạt được.
   - Mức độ hoàn thành.

4. PHẢN HỒI CẢI THIỆN
   - Điểm mạnh.
   - Điểm yếu.
   - Lỗi cần sửa.
   - Hướng khắc phục cụ thể.

5. CÂU HỎI KIỂM TRA
   - Đặt 2 câu hỏi vận dụng kiến thức.

**PHONG CÁCH (STYLE)**

Sử dụng tiếng Việt rõ ràng, dễ hiểu, có tính hướng dẫn. Trình bày khoa học, có bảng biểu khi cần thiết. Phản hồi mang tính xây dựng, không chỉ đưa ra điểm số mà phải giúp người học hiểu và tiến bộ.

