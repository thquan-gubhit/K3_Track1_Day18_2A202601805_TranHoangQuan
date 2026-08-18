# Hypothesis Problem nhóm tiếp tục

Khi đang theo dõi một buổi học có nội dung mới, nặng hoặc được giảng với tốc độ nhanh, learner gặp khó khăn trong việc hiểu bài và tiếp tục theo kịp mạch giảng vì không hiểu một phần kiến thức nhưng không hỏi hoặc không nhận được hỗ trợ ngay, dẫn đến phải tự tra cứu, bỏ lỡ nội dung tiếp theo, mất thêm thời gian học lại hoặc làm bài chậm hơn.

## Evidence ban đầu hỗ trợ giả thuyết:

Cả ba learner đều mô tả tình huống gặp phần kiến thức khó ngay trong lúc bài giảng đang tiếp tục. Họ thường không hỏi giảng viên ngay mà tự tra cứu bằng Google, ChatGPT hoặc học lại ở nhà. Các hậu quả được ghi nhận gồm mất flow bài giảng, bỏ lỡ kiến thức phía sau, phải dành thêm thời gian tự học và làm bài tập chậm hơn. Một learner cho biết khi chưa hiểu phần trước thì các khái niệm sau trở nên khó hiểu hơn.

## Điều vẫn chưa được chứng minh:

Nhóm chưa chứng minh được instructor có thực sự không nhận ra learner đang gặp khó khăn hay không; việc hỗ trợ sớm có chắc chắn giúp learner theo kịp bài hơn hay không; và những tín hiệu như xem lại slide, ghi chú, đổi đáp án hoặc trò chuyện với AI có đủ chính xác để xác định learner nào đang cần hỗ trợ. Hiện tại, evidence chủ yếu đến từ phía learner, chưa có instructor-side evidence.

# three option

- Option A: Learner cần biết thông tin mình gửi sẽ được chia sẻ với ai và có thể rút hoặc cập nhật check-in.
- Option B: Feedback “cảnh báo hữu ích/không hữu ích” không nên tự động thay đổi rule trong phiên hiện tại. Việc thay đổi rule cần được review riêng.
- Option C: Feedback của instructor không nên được mặc định dùng để huấn luyện hoặc thay đổi mô hình nếu chưa được thông báo. Learner cần biết những dữ liệu nào được phân tích, mục đích sử dụng, người có quyền xem và cách rút quyền đối với dữ liệu không bắt buộc.

# Những thứ phải giữ nguyên

| Thành phần               | Quyết định chung cho A/B/C                                                                                                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Target user**          | **Instructor hoặc coach** — người xem thông tin và quyết định có hỗ trợ learner hay không                                                                                                        |
| **Situation**            | Trong hoặc ngay sau một phiên học, một learner gặp khó khăn ở một phần kiến thức nhưng chưa trực tiếp yêu cầu hỗ trợ                                                                             |
| **Task**                 | Xác định learner có cần được chú ý hoặc hỗ trợ thêm không, đang gặp khó khăn ở đâu và nên thực hiện hành động nào                                                                                |
| **Desired outcome**      | Instructor đưa ra quyết định hỗ trợ kịp thời và có căn cứ, đồng thời hạn chế làm gián đoạn những learner vẫn có thể tự giải quyết                                                                |
| **Content/data fixture** | Cùng một tình huống: learner gặp khó ở phần RAG/AI Agent; xem lại slide, dừng lâu, thay đổi đáp án, ghi chú “Chưa hiểu”, sử dụng AI Chat và tự tra cứu nhưng vẫn khó theo kịp nội dung tiếp theo |

# Ba solution hypotheses

| Thành phần             | Option A — Learner Check-in                                                                                                                                  | Option B — Rule-based Alert                                                                             | Option C — AI Support Radar                                                                                                                                              |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Solution mechanism** | Learner chủ động báo mức độ hiểu và yêu cầu hỗ trợ                                                                                                           | Hệ thống sử dụng các điều kiện và ngưỡng được định nghĩa trước để tạo cảnh báo                          | AI kết hợp nhiều tín hiệu để nhận định learner có thể cần hỗ trợ                                                                                                         |
| **User làm gì?**       | Instructor xem check-in do learner gửi, đọc phần learner đánh dấu chưa hiểu và quyết định phản hồi                                                           | Instructor xem cảnh báo, kiểm tra các tín hiệu đã kích hoạt rule và quyết định có can thiệp không       | Instructor xem learner được AI đề xuất, nội dung khó khăn, các tín hiệu liên quan và hành động hỗ trợ được gợi ý; sau đó xác nhận hoặc bỏ qua                            |
| **AI làm gì?**         | Không sử dụng AI                                                                                                                                             | Không sử dụng AI; hệ thống chỉ áp dụng các rule cố định                                                 | Tổng hợp tín hiệu, ước lượng khả năng learner cần hỗ trợ, giải thích căn cứ và đề xuất hành động                                                                         |
| **Trigger**            | Learner chọn “Chưa hiểu”, gửi check-in hoặc yêu cầu hỗ trợ                                                                                                   | Một ngưỡng được kích hoạt, ví dụ sai nhiều lần, xem lại slide nhiều lần hoặc đánh dấu “Chưa hiểu”       | Sau phiên học hoặc khi hệ thống thu thập đủ nhiều tín hiệu liên quan                                                                                                     |
| **Trade-off chính**    | Minh bạch, ít suy đoán và tôn trọng quyền chủ động của learner; nhưng có thể bỏ sót người ngại hỏi, không nhận ra mình hiểu sai hoặc không muốn báo khó khăn | Dễ giải thích và nhất quán; nhưng rule cứng có thể tạo cảnh báo sai hoặc bỏ sót các trường hợp phức tạp | Có thể nhận ra các pattern phức tạp và giảm công sức tổng hợp; nhưng có rủi ro suy luận sai, khó giải thích, ảnh hưởng quyền riêng tư và khiến instructor quá tin vào AI |

# Solution hypothesis của từng option

Option A:

Nếu learner có một cách đơn giản để chủ động báo phần chưa hiểu, instructor sẽ có đủ thông tin để xác định và hỗ trợ những learner đang thực sự muốn được giúp.

Option B:

Nếu hệ thống cảnh báo instructor khi các tín hiệu học tập vượt qua những ngưỡng rõ ràng, instructor sẽ phát hiện sớm hơn các learner có khả năng đang mất flow.

Option C:

Nếu AI tổng hợp nhiều tín hiệu và giải thích vì sao một learner có thể cần hỗ trợ, instructor sẽ xác định và ưu tiên các trường hợp cần chú ý nhanh hơn so với tự xem từng nguồn dữ liệu.

Ba option này cùng giải một task nhưng kiểm tra ba niềm tin khác nhau:

A: Learner có thể và sẽ tự báo khi cần giúp.
B: Difficulty đáng chú ý có thể được xác định bằng rule rõ ràng.
C: Cần AI để hiểu các tín hiệu phức tạp và ưu tiên hỗ trợ.

## A khác B vì A dựa vào learner chủ động tạo tín hiệu và yêu cầu hỗ trợ, còn B tự khởi tạo cảnh báo khi các điều kiện định sẵn được kích hoạt.

## B khác C vì B chỉ áp dụng các rule cố định và minh bạch, còn C dùng AI để tổng hợp nhiều tín hiệu, suy luận mức độ cần hỗ trợ và đề xuất hành động.

## A khác C vì A trao quyền khởi tạo hoàn toàn cho learner, còn C để AI chủ động phát hiện trường hợp có thể cần hỗ trợ rồi chuyển cho instructor xem xét.

A: USER CREATES / INITIATES
→ B: SYSTEM INITIATES BY FIXED RULES, USER REVIEWS
→ C: AI CREATES / INITIATES, USER REVIEWS
