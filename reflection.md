# Individual reflection — Nguyễn Minh Quân (AI20K001)

## 1. Role
Prompt engineer. Phụ trách thiết kế flow chatbot và viết system prompt.
Visualizing: thiết kế powerpoint và SPEC.

## 2. Đóng góp cụ thể
- Thiết kế conversation flow 5 bước (hỏi vị trí đau → thời gian → mức độ → tiền sử → gợi ý)
- Thiết kế Mini AI SPEC
- Vẽ poster layout cho demo, canvas và slide
- Viết problem statement để triển khai bot AI

## 3. SPEC mạnh/yếu
- Mạnh nhất (Failure Modes): Xây dựng kịch bản xử lý chặt chẽ cho trường hợp "triệu chứng mơ hồ". Thay vì đoán mò chuyên khoa (gây rủi ro), AI sẽ kích hoạt luồng câu hỏi làm rõ (follow-up) hoặc chuyển hướng nhân viên hỗ trợ nếu cần thiết.
- Yếu nhất: ROI — Cả 3 kịch bản (Thận trọng, Thực tế, Lạc quan) hiện tại thực chất chỉ khác nhau về số lượng người dùng (user base) mà chưa có sự thay đổi về các giả định cốt lõi (assumptions).
                _ Thiếu chiều sâu vận hành: Các con số như "giảm 15% tải trọng" hay "tăng 10% doanh thu" mới chỉ dừng lại ở mức ước tính cảm tính, chưa gắn liền với quy mô triển khai cụ thể của hệ thống Vinmec.

## 4. Đóng góp khác
- Test prompt với 5 triệu chứng khác nhau.
- Tổng quát SPEC để nhóm cùng nhau demo.

## 5. Điều học được
Trước hackathon nghĩ precision và recall chỉ là metric kỹ thuật.
Sau khi thiết kế AI triage mới hiểu: chọn recall cao hơn cho khoa cấp cứu
(bỏ sót nguy hiểm hơn false alarm) nhưng precision cao hơn cho khoa chuyên sâu
(gợi ý sai gây lãng phí thời gian bệnh nhân). Metric là product decision,
không chỉ engineering decision. Không nên sử dụng mô hình rule-based để chuẩn đoán chi tiết bệnh.

## 6. Nếu làm lại
Sẽ test prompt sớm hơn — ngày đầu chỉ viết SPEC, đến trưa D6 mới bắt đầu test prompt.
Làm system prompt tốt hơn để AI không bị lệch đề và trả lời lung tung.

## 7. AI giúp gì / AI sai gì
- **Giúp:** dùng Claude để brainstorm failure modes — nó gợi ý được "drug interaction"
  mà nhóm không nghĩ ra. Dùng Gemini để test prompt nhanh qua AI Studio.
- **Sai/mislead:** Claude gợi ý thêm feature "đặt lịch khám" vào chatbot —
  nghe hay nhưng scope quá lớn cho hackathon.Cần hoàn thiện luồng đặt lịch vì đang bị lỗi.
  Bài học: AI brainstorm và scope tốt nhưng chưa chuẩn và đôi khi bị hallucinate.
