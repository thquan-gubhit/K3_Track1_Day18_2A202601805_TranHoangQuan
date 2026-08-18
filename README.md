# AI Support Radar — Day 18

## 1. Thông tin cá nhân và nhóm

- **MHV:** 2A202601805
- **Họ và tên:** Trần Hoàng Quân
- **Tên nhóm:** `[Bổ sung tên nhóm]`
- **Case:** Case C — AI Support Radar

### Thành viên nhóm

| STT | Họ và tên                | MHV             |
| --: | ------------------------ | --------------- |
|   1 | Trần Hoàng Quân          | 2A202601805     |
|   2 | `[Bổ sung thành viên 2]` | `[Bổ sung MHV]` |
|   3 | `[Bổ sung thành viên 3]` | `[Bổ sung MHV]` |

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

**Prototype:** `[Bổ sung link Option A]`

### Option B — Rule-based Alert

Hệ thống tạo cảnh báo khi các điều kiện định trước được kích hoạt, ví dụ learner dừng lâu ở một slide, đổi đáp án nhiều lần, trả lời sai quiz hoặc đánh dấu “Chưa hiểu”. Instructor xem rule, ngưỡng và dữ liệu liên quan trước khi quyết định.

**Solution hypothesis:**

> Nếu hệ thống cảnh báo instructor khi các tín hiệu học tập vượt qua những ngưỡng rõ ràng, instructor sẽ phát hiện sớm hơn các learner có khả năng đang mất flow.

**Prototype:** `[Bổ sung link Option B]`

### Option C — AI Support Radar

AI tổng hợp nhiều tín hiệu để nhận định learner có thể cần hỗ trợ, xác định nội dung learner có thể đang gặp khó khăn, trình bày evidence và đề xuất một hành động hỗ trợ. Instructor là người review và đưa ra quyết định cuối cùng.

**Solution hypothesis:**

> Nếu AI tổng hợp nhiều tín hiệu và giải thích vì sao một learner có thể cần hỗ trợ, instructor sẽ xác định và ưu tiên các trường hợp cần chú ý nhanh hơn so với tự xem từng nguồn dữ liệu.

**Prototype:** `[Bổ sung link Option C]`

### Prototype chung

- **Link prototype A/B/C:** `[Bổ sung link prototype chung]`
- **Trạng thái:** Đã build ba micro-prototype, chưa thực hiện prototype testing.
- **Dữ liệu sử dụng:** Canned data và canned AI output, chưa tích hợp model hoặc API thật.

---

## 4. Đóng góp của tôi trong nhóm

Trong quá trình thực hiện, tôi đã tham gia các công việc sau:

- Chuẩn bị task và kịch bản test.
- Facilitate một phiên test A/B/C.
- Quan sát hành vi của tester.
- Ghi exact quote và quyết định ở từng option.
- Hoàn thành prototype-feedback-note.md.
- Tham gia xác định scope cho ba micro-prototype theo luồng:

```text
COMMON CONTEXT
      ↓
CRITICAL INTERACTION
      ↓
RESULT / USER DECISION
```

- Tham gia build ba micro-prototype.

Do nhóm mới hoàn thành giai đoạn build, tôi chưa thực hiện facilitation, observation hoặc tổng hợp feedback từ prototype testing.

---

## 5. Prototype Feedback

### Trạng thái hiện tại

Nhóm đã hoàn thành ba micro-prototype nhưng **chưa tiến hành test với tester**. Vì vậy, phần này chưa có observation hoặc feedback thực tế.

### Observation từ phiên tôi facilitate

> Chưa có — tôi chưa facilitate phiên prototype testing.

### Three-feedback synthesis

> Chưa có — nhóm chưa thu thập đủ ba nguồn feedback để tổng hợp pattern giữa các phiên.

### Next Change

> Chưa quyết định. Nhóm sẽ chỉ xác định thay đổi tiếp theo sau khi quan sát tester tự thực hiện cùng một task trên ba option A/B/C.

Các điểm dự kiến cần quan sát trong phiên test gồm:

- Tester có hiểu vì sao thông tin hoặc cảnh báo xuất hiện không.
- Evidence hiện có đã đủ để tester ra quyết định chưa.
- Tester có kiểm tra dữ liệu gốc trước khi liên hệ learner không.
- Tester có biết cách dismiss, edit, reject hoặc quay lại task ban đầu không.
- Option nào giúp tester ra quyết định mà không cần facilitator giải thích.

### Still Unproven

Các nội dung sau vẫn chưa được chứng minh:

- Instructor có thực sự gặp khó khăn trong việc nhận biết learner cần hỗ trợ hay không.
- Instructor thiếu visibility hay đã biết learner cần hỗ trợ nhưng thiếu thời gian và nguồn lực để hành động.
- Learner có chủ động sử dụng check-in khi gặp khó khăn hay không.
- Các rule cố định có phân biệt được difficulty đáng chú ý với hành vi học tập bình thường hay không.
- AI có thể tổng hợp tín hiệu chính xác và cung cấp evidence đủ đáng tin cậy hay không.
- Nhận định của AI có thực sự giúp instructor ra quyết định nhanh hoặc tốt hơn không.
- Tester có quá tin vào AI hoặc các cảnh báo tự động hay không.
- Learner có chấp nhận việc các tín hiệu học tập của mình được phân tích và chia sẻ với instructor hay không.
- Việc hỗ trợ sớm có thực sự làm giảm tình trạng mất flow, bỏ lỡ kiến thức và phải học lại hay không.

---

## 6. AI Support Log

AI được sử dụng như một công cụ hỗ trợ brainstorm, cấu trúc nội dung và rà soát tài liệu. Quyết định cuối cùng do nhóm tự xem xét và chỉnh sửa.

### AI đã hỗ trợ gì?

AI đã hỗ trợ nhóm:

- Giải thích các khái niệm như solution, directive, capability, actor, situation, job, pain, evidence, workaround và consequence.
- Chuyển AI Support Radar từ một solution cụ thể thành capability trung tính.
- Làm rõ change chain từ solution đến outcome.
- Xác định các actor liên quan gồm learner, instructor và coach.
- Xây dựng Situation & Job và JTBD Hypothesis.
- Viết hai Pain Hypotheses cạnh tranh.
- Xây dựng bảng evidence làm giả thuyết mạnh hơn hoặc yếu đi.
- Brainstorm Solution Parking Lot với cả hướng sử dụng và không sử dụng AI.
- Soạn và rút gọn Conversation Guide.
- Phân tích ba nội dung phỏng vấn learner.
- Tách riêng:
  - Lời và hành động thực tế của learner.
  - Phần diễn giải của nhóm.
  - Workaround.
  - Consequence.
  - Evidence trái giả thuyết.

- Hỗ trợ chốt Hypothesis Problem.
- Xây dựng ba solution hypotheses A/B/C.
- Xây dựng Human–AI Decision Table.
- Xác định common context, content fixture, prototype scope và prototype annotation.
- Hỗ trợ cấu trúc tài liệu README.

### AI sai hoặc hời hợt ở đâu?

Một số hạn chế trong đầu ra của AI:

- Một số câu trả lời dài hơn mức cần thiết.
- Có lúc AI diễn giải hoặc kết luận mạnh hơn evidence thực tế từ phỏng vấn.
- Có lúc AI biến một nhận xét của learner thành finding chung cho nhiều learner.
- AI từng đề xuất bổ sung phần **support threshold**, trong khi nhóm không chọn đưa phần này vào phiên bản cuối.
- Một số đề xuất ban đầu tập trung nhiều vào việc phát hiện learner sau phiên học, trong khi evidence cho thấy difficulty thường xuất hiện ngay trong lúc bài giảng đang diễn ra.
- AI có xu hướng phát triển thêm nhiều màn hình, trạng thái hoặc tiêu chí hơn phạm vi micro-prototype cần test.
- AI chưa thể thay thế evidence thực tế từ instructor/coach hoặc prototype tester.

### Tôi đã tự kiểm tra và sửa như thế nào?

Tôi và nhóm đã:

- Đối chiếu nội dung AI tổng hợp với transcript và nội dung phỏng vấn gốc.
- Tách rõ exact quote, hành vi thực tế và phần suy luận của nhóm.
- Không coi một problem statement hợp lý là evidence.
- Loại bỏ hoặc giảm mức độ chắc chắn của các kết luận chưa được dữ liệu hỗ trợ.
- Ghi rõ evidence hiện tại chủ yếu đến từ learner và instructor-side job chưa được kiểm chứng.
- Mở rộng phạm vi nghiên cứu từ “sau phiên học” thành “trong hoặc ngay sau phiên học” dựa trên dữ liệu phỏng vấn.
- Loại bỏ phần support threshold khỏi Conversation Guide phiên bản cuối.
- Giữ ba option ở cùng một task và content fixture để tránh so sánh những solution giải các vấn đề khác nhau.
- Giới hạn mỗi option trong 2–3 trạng thái, chỉ làm khác critical interaction.
- Giữ instructor là người review và quyết định cuối cùng, thay vì để AI tự động liên hệ learner.
- Không đưa ra kết luận option nào tốt hơn vì prototype chưa được test.
