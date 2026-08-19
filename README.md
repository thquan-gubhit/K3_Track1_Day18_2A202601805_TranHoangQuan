# AI Support Radar — Day 18

## 1. Thông tin cá nhân và nhóm

- **MHV:** 2A202601805
- **Họ và tên:** Trần Hoàng Quân
- **Tên nhóm:** 1
- **Case:** Case C — AI Support Radar

### Thành viên nhóm

| STT | Họ và tên        | MHV         |
| --: | ---------------- | ----------- |
|   1 | Trần Hoàng Quân  | 2A202601805 |
|   2 | Trần Thị Hoa Mai | 2A202601317 |

---

## 2. Hypothesis Problem

> Khi **đang theo dõi một buổi học có nội dung mới, nặng hoặc được giảng với tốc độ nhanh**, **learner** gặp khó khăn trong việc **hiểu bài và tiếp tục theo kịp mạch giảng** vì **không hiểu một phần kiến thức nhưng không hỏi hoặc không nhận được hỗ trợ ngay**, dẫn đến **phải tự tra cứu, bỏ lỡ nội dung tiếp theo, mất thêm thời gian học lại hoặc làm bài chậm hơn**.

Hypothesis Problem này được nhóm sử dụng làm điểm xuất phát trong Day 18. Evidence ban đầu đến từ ba cuộc phỏng vấn learner, trong đó các workaround được nhắc đến gồm tự tra cứu bằng Google, ChatGPT hoặc học lại ở nhà.

Hiện tại, nhóm chưa chứng minh được instructor có thực sự không nhận ra learner đang gặp khó khăn hay không và việc hỗ trợ sớm có chắc chắn cải thiện kết quả học tập hay không.

---

## 3. Three Solution Options

Ba option cùng sử dụng một target user, situation, task, desired outcome và content fixture. Điểm khác nhau chính nằm ở cơ chế khởi tạo thông tin hỗ trợ.

### Option A — Learner Check-in

Learner chủ động đánh dấu phần chưa hiểu hoặc gửi yêu cầu hỗ trợ. Instructor xem thông tin learner cung cấp và quyết định có liên hệ, gửi tài liệu, để lại xử lý sau hoặc bỏ qua hay không.

**Solution hypothesis:**

> Nếu learner có một cách đơn giản để chủ động báo phần chưa hiểu, instructor sẽ có đủ thông tin để hỗ trợ những learner đang thực sự muốn được giúp.

### Option B — Rule-based Alert

Hệ thống tạo cảnh báo khi các điều kiện định trước được kích hoạt, ví dụ learner dừng lâu ở một slide, đổi đáp án nhiều lần, trả lời sai quiz hoặc đánh dấu “Chưa hiểu”. Instructor xem rule, ngưỡng và dữ liệu liên quan trước khi quyết định.

**Solution hypothesis:**

> Nếu hệ thống cảnh báo instructor khi các tín hiệu học tập vượt qua những ngưỡng rõ ràng, instructor sẽ phát hiện sớm hơn các learner có khả năng đang mất flow.

### Option C — AI Support Radar

AI tổng hợp nhiều tín hiệu để nhận định learner có thể cần hỗ trợ, xác định nội dung learner có thể đang gặp khó khăn, trình bày evidence và đề xuất một hành động hỗ trợ. Instructor là người review và đưa ra quyết định cuối cùng.

**Solution hypothesis:**

> Nếu AI tổng hợp nhiều tín hiệu và giải thích vì sao một learner có thể cần hỗ trợ, instructor sẽ xác định và ưu tiên các trường hợp cần chú ý nhanh hơn so với tự xem từng nguồn dữ liệu.

### Prototype chung

- **Link prototype A/B/C:**https://thquan-gubhit.github.io/day18_prototype/
- **Trạng thái:** Đã build ba micro-prototype, chưa thực hiện prototype testing.
- **Dữ liệu sử dụng:** Canned data và canned AI output, chưa tích hợp model hoặc API thật.

---

## 4. Đóng góp của tôi trong nhóm

Tôi phụ trách chính phần problem discovery, phỏng vấn và tổng hợp evidence, bao gồm:

- Phân tích solution directive ban đầu và chuyển thành capability trung tính.
- Tham gia xác định actor, situation, job, pain và consequence.
- Xây dựng và điều chỉnh Conversation Guide dành cho learner.
- Thực hiện phỏng vấn và ghi nhận các tình huống thực tế của learner.
- Bóc tách dữ liệu phỏng vấn thành:
  - Situation và job.
  - Hành vi thực tế.
  - Khó khăn và workaround.
  - Hậu quả hoặc chi phí.
  - Evidence trái giả thuyết và exact quote.
- Tham gia chốt Hypothesis Problem dùng cho Day 18.
- Tham gia xác định ba solution options A/B/C.
- Chuẩn bị shared context, task và content fixture dùng chung cho prototype.
- Facilitate các phiên prototype test với Lab Coach.
- Ghi nhận observation, lựa chọn của tester và evidence chống lại kỳ vọng.
- Tham gia tổng hợp feedback, Next Change và Still Unproven.

---

## 5. Prototype Feedback

### Trạng thái hiện tại

Nhóm đã hoàn thành ba micro-prototype A/B/C và tiến hành **ba phiên prototype testing với Lab Coach**.

Ba tester gồm:

- Nguyễn Thành Đạt — Lab Coach.
- Nguyễn Thành Tài — Lab Coach.
- Võ Huyền Khánh Mây — Lab Coach.

Cả ba tester đều thực hiện theo thứ tự **A → B → C** và cùng được giao task đánh giá tình trạng learner để quyết định có cần hỗ trợ hay không.

### Observation từ phiên tôi facilitate

Một số observation chính từ ba phiên test:

- Tester đều bắt đầu bằng việc đọc **context, task hoặc tình trạng learner** trước khi đưa ra quyết định.
- Cả ba tester đều đọc evidence được cung cấp trong các option thay vì chỉ dựa vào cảnh báo hoặc đề xuất.
- Hai tester có biểu hiện do dự khi lựa chọn phương án hỗ trợ cho learner.
- Một tester ban đầu hiểu nhầm A/B/C là **ba lựa chọn trong cùng một flow**, thay vì ba solution prototypes độc lập để so sánh.
- Khi chưa chắc chắn, tester có xu hướng đọc thêm evidence trước khi đưa ra quyết định.
- Không tester nào chọn duy nhất một option:
  - Tester 1 chọn **A + C**.
  - Tester 2 chọn **B + C**.
  - Tester 3 chọn **A + B**.

- Tester chỉ ra rằng một số behavioral signal có thể là nhiễu. Ví dụ, việc learner dừng lâu ở một slide có thể do rời máy chứ không nhất thiết vì không hiểu.
- Hai tester nhấn mạnh rằng khi đã có tín hiệu learner gặp khó khăn, việc hỗ trợ nên diễn ra **ngay trong buổi học**, thay vì đợi đến sau phiên học.
- Một tester không hoàn toàn tin vào AI inference vì chưa rõ AI sử dụng threshold và các tín hiệu như thế nào để xác định learner cần hỗ trợ.

### Three-feedback synthesis

Ba phiên test cho thấy một số pattern chung:

1. **Evidence là yếu tố quan trọng trước khi instructor ra quyết định.**
   Cả ba tester đều đọc evidence và sử dụng nó để đánh giá tình trạng learner thay vì chỉ tin vào cảnh báo hoặc đề xuất.

2. **Không có một option đơn lẻ được ưu tiên tuyệt đối.**
   Cả ba tester đều chọn kết hợp hai mechanism khác nhau. A, B và C đều xuất hiện trong 2/3 lựa chọn, cho thấy mỗi mechanism có điểm mạnh và hạn chế riêng.

3. **Tester ưu tiên khả năng phát hiện learner cần hỗ trợ sớm.**
   Một số tester chấp nhận khả năng xuất hiện false positive nếu đổi lại giảm nguy cơ bỏ sót learner thực sự cần hỗ trợ.

4. **Rule-based được đánh giá là dễ kiểm soát hơn AI trong một số trường hợp.**
   Tester quan tâm đến việc nhìn thấy threshold và nguyên nhân cảnh báo. Với AI, có lo ngại về việc không biết hệ thống suy luận dựa trên tiêu chí nào.

5. **Một số signal có thể không phản ánh difficulty thực sự.**
   Ví dụ thời gian dừng lâu trên slide có thể là tín hiệu nhiễu, nên không nên coi một signal riêng lẻ là đủ để kết luận learner cần hỗ trợ.

6. **Thời điểm hỗ trợ là một finding đáng chú ý.**
   Hai trong ba tester cho rằng khi đã có evidence đủ rõ, instructor nên kiểm tra hoặc hỗ trợ learner ngay trong lúc buổi học đang diễn ra thay vì chờ đến sau buổi học.

### Next Change

> **Chuyển critical moment của prototype từ sau buổi học sang ngay trong lúc learner đang gặp khó khăn trên lớp, đồng thời giữ evidence đủ rõ để instructor tự quyết định có nên hỏi hoặc hỗ trợ learner ngay hay không.**

### Evidence dẫn tới Next Change

Hai trong ba tester trực tiếp nhấn mạnh rằng khi đã xuất hiện tín hiệu learner có thể đang gặp khó khăn, instructor nên kiểm tra hoặc hỗ trợ **ngay tại thời điểm đó**, không nên đợi đến sau phiên học.

Ngoài ra, tester cũng chỉ ra rằng một số signal có thể là nhiễu, nên hệ thống không nên tự động kết luận hoặc can thiệp. Instructor vẫn cần xem evidence và giữ quyền quyết định cuối cùng.

### Still Unproven

Sau ba phiên feedback, nhóm vẫn chưa chứng minh được:

- Combination nào giữa A/B/C thực sự hiệu quả hơn.
- Một option đơn lẻ có đủ để hỗ trợ instructor hay cần kết hợp nhiều mechanism.
- Learner có chủ động sử dụng check-in trong tình huống thực tế hay không.
- Signal nào đủ đáng tin và signal nào chủ yếu là nhiễu.
- Threshold nào phù hợp để rule-based alert không tạo quá nhiều false positive.
- AI có thể tổng hợp các signal chính xác và đáng tin hơn rule-based hay self-report hay không.
- Instructor có thể hiểu và kiểm tra reasoning của AI đủ tốt để không phụ thuộc quá mức vào AI.
- Việc can thiệp ngay trong lớp có thực sự giúp learner theo kịp bài tốt hơn hay có thể làm gián đoạn learner hoặc lớp học.
- Learner có chấp nhận việc các tín hiệu học tập của mình được phân tích và chia sẻ với instructor hay không.
- Các kết quả từ ba Lab Coach có generalize sang instructor hoặc coach khác hay không.

---

## 6. AI Support Log

AI được sử dụng như một công cụ hỗ trợ brainstorm, cấu trúc nội dung, phân tích evidence và rà soát tài liệu. Các quyết định cuối cùng được tôi và nhóm tự kiểm tra và điều chỉnh dựa trên dữ liệu thực tế.

### AI đã hỗ trợ gì?

AI đã hỗ trợ nhóm trong các giai đoạn sau:

- Giải thích các khái niệm như solution, directive, capability, actor, situation, job, pain, evidence, workaround và consequence.
- Chuyển AI Support Radar từ một solution cụ thể thành capability trung tính.
- Làm rõ change chain từ solution đến outcome.
- Xác định các actor liên quan gồm learner, instructor và coach.
- Xây dựng Situation & Job và JTBD Hypothesis.
- Viết hai Pain Hypotheses cạnh tranh.
- Xây dựng bảng evidence làm giả thuyết mạnh hơn hoặc yếu đi.
- Brainstorm Solution Parking Lot với cả hướng sử dụng AI và không sử dụng AI.
- Soạn, rút gọn và điều chỉnh Conversation Guide.
- Phân tích ba cuộc phỏng vấn learner.
- Hỗ trợ tách riêng:
  - Lời và hành động thực tế của learner.
  - Phần diễn giải của nhóm.
  - Khó khăn và workaround.
  - Consequence.
  - Evidence trái giả thuyết.
  - Exact quote đáng chú ý.

- Hỗ trợ chốt Hypothesis Problem dùng trong Day 18.
- Xây dựng ba solution hypotheses:
  - A — Learner Check-in.
  - B — Rule-based Alert.
  - C — AI Support Radar.

- Xây dựng Human–AI Decision Table.
- Xác định common context, content fixture, prototype scope và prototype annotation.
- Hỗ trợ xây dựng micro-prototype HTML/CSS/JavaScript ban đầu.
- Điều chỉnh prototype để thông tin learner chỉ xuất hiện sau khi tester chọn từng option.
- Hỗ trợ giải thích các trường cần ghi trong Prototype Feedback Note như First Action, Control/Recovery và Evidence chống lại kỳ vọng.
- Hỗ trợ tổng hợp ba phiên prototype feedback thành các pattern chung.
- Gợi ý Next Change và danh sách Still Unproven dựa trên evidence từ ba tester.
- Hỗ trợ cấu trúc và cập nhật README.

### AI sai hoặc hời hợt ở đâu?

Một số hạn chế trong đầu ra của AI:

- Một số câu trả lời dài và mở rộng nhiều hơn phạm vi cần thiết.
- Có lúc AI diễn giải hoặc kết luận mạnh hơn evidence thực tế từ phỏng vấn.
- Có lúc AI biến một nhận xét của một learner thành finding chung trước khi kiểm tra xem pattern có lặp lại hay không.
- AI từng đề xuất bổ sung phần **support threshold**, trong khi nhóm không chọn đưa nội dung này vào phiên bản cuối.
- Một số đề xuất ban đầu tập trung vào việc phát hiện learner **sau phiên học**, trong khi evidence từ learner và prototype tester đều cho thấy critical moment có thể nằm ngay trong lúc buổi học đang diễn ra.
- AI có xu hướng đề xuất thêm màn hình hoặc trạng thái nhiều hơn phạm vi micro-prototype cần test.
- Khi phân tích prototype feedback, AI ban đầu có xu hướng tìm một option nổi trội, trong khi dữ liệu thực tế cho thấy cả ba tester đều muốn kết hợp hai mechanism và chưa có option thắng rõ ràng.
- AI không thể tự xác định signal hoặc threshold nào thực sự chính xác nếu chưa có dữ liệu thực tế để kiểm chứng.

### Tôi đã tự kiểm tra và sửa như thế nào?

Tôi và nhóm đã:

- Đối chiếu nội dung AI tổng hợp với transcript và nội dung phỏng vấn gốc.
- Tách rõ exact quote, hành vi thực tế và phần suy luận của nhóm.
- Không coi một problem statement hợp lý là evidence.
- Chỉ xem một pattern là đáng chú ý khi có dữ liệu thực tế hỗ trợ.
- Loại bỏ hoặc giảm mức độ chắc chắn của các kết luận chưa được chứng minh.
- Ghi rõ giới hạn của learner-side evidence trước khi có dữ liệu từ Lab Coach.
- Mở rộng phạm vi từ “sau phiên học” thành “trong hoặc ngay sau phiên học” dựa trên evidence thực tế.
- Loại bỏ phần support threshold khỏi Conversation Guide phiên bản cuối.
- Giữ A/B/C cùng một task và context để việc so sánh tập trung vào solution mechanism.
- Giới hạn mỗi option ở critical interaction cần test thay vì xây toàn bộ product.
- Giữ instructor là người review evidence và đưa ra quyết định cuối cùng.
- Điều chỉnh prototype để không hiển thị toàn bộ thông tin learner ngay từ common context; evidence chỉ xuất hiện khi tester vào từng option.
- Không kết luận A, B hoặc C là option tốt nhất vì ba tester đều chọn các combination khác nhau.
- Không coi một behavioral signal như thời gian xem slide lâu là bằng chứng chắc chắn learner gặp khó khăn, sau khi tester chỉ ra khả năng signal này bị nhiễu.
- Chọn Next Change dựa trên feedback lặp lại từ tester: đưa critical interaction về **ngay trong lúc học**, thay vì tiếp tục giữ assumption rằng hỗ trợ nên diễn ra sau phiên học.
