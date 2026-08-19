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

### AI đã giúp tôi ở đâu?

AI hỗ trợ gợi ý và rà soát ba solution mechanisms A/B/C để bảo đảm chúng khác nhau về cách khởi tạo và role split; tạo content fixture và canned AI output dùng chung cho prototype; hỗ trợ viết code prototype HTML/CSS/JavaScript; và gợi ý các câu hỏi trung tính để dùng khi test. AI cũng giúp kiểm tra scope để prototype chỉ tập trung vào critical interaction.

### AI sai, hời hợt hoặc làm các options giống nhau ở đâu?

Ban đầu AI có xu hướng mở rộng prototype thành quá nhiều màn hình và diễn giải một số evidence mạnh hơn dữ liệu thực tế. AI cũng từng đề xuất thêm “support threshold” dù nhóm không cần phần này, và một số phiên bản ban đầu chưa làm A/B/C khác nhau đủ rõ về mechanism.

### Tôi đã tự sửa hoặc quyết định lại điều gì?

Tôi đối chiếu lại transcript và feedback gốc, giữ nguyên quote và observation của tester, đồng thời tách rõ evidence với phần diễn giải của nhóm. Tôi bỏ các kết luận chưa có dữ liệu hỗ trợ, loại bỏ phần support threshold, chỉnh lại A/B/C để khác nhau rõ về mechanism và giữ cùng common context. Việc tester chọn option nào, Next Change và các kết luận cuối đều do tester và nhóm quyết định, không dùng AI để quyết định thay.
