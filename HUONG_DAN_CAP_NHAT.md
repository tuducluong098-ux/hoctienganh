# 📖 HƯỚNG DẪN CẬP NHẬT BÀI HỌC & ĐỀ THI MỚI

Trang web **"HỌC TIẾNG ANH 2 TRIỆU 3"** được thiết kế dưới dạng Single-Page tĩnh, toàn bộ dữ liệu (bài đọc, tranh ảnh, từ vựng, email, bài luận) đều được tổ chức dạng danh sách (Array) cực kỳ ngăn nắp bên trong file `index.html`.

Dưới đây là 2 cách cập nhật bài tập mới dễ nhất:

---

## 🤖 CÁCH 1: Nhờ AI Cập Nhật Hộ (Khuyên dùng - Nhanh nhất)

Bạn không cần phải tự sửa mã code. Bất cứ khi nào bạn hoặc người yêu có thêm đề thi mới:

1. **Chụp ảnh màn hình** đề thi, hoặc copy văn bản đề bài.
2. Gửi vào cửa sổ chat với AI (Antigravity hoặc ChatGPT) kèm câu lệnh đơn giản:
   > *"Cập nhật câu hỏi Speaking/Writing này vào repo hoctienganh giúp tôi: [Dán nội dung đề bài tại đây]"*
3. AI sẽ tự động:
   - Trích xuất từ vựng, phiên âm IPA chuẩn.
   - Soạn bài trả lời mẫu đạt điểm tối đa (Band 3 - Band 4).
   - Tự commit và đẩy (push) lên GitHub.
4. Sau 1 phút, bạn gái chỉ cần tải lại trang web là có ngay bài học mới!

---

## ✏️ CÁCH 2: Tự Chỉnh Sửa Trực Tiếp Trên GitHub Web (1 Phút)

Bạn có thể chỉnh sửa trực tiếp trên điện thoại hoặc máy tính mà không cần cài đặt bất kỳ phần mềm lập trình nào:

### Bước 1: Mở file `index.html` trên GitHub
Truy cập đường dẫn:  
👉 **`https://github.com/tuducluong098-ux/hoctienganh/blob/main/index.html`**

### Bước 2: Bấm vào biểu tượng cây bút ✏️ (*Edit this file*) ở góc trên bên phải.

### Bước 3: Tìm đến phần dữ liệu bạn muốn thêm:

#### 1. Thêm bài đọc Part 1 Speaking:
Tìm từ khóa: `// DATA: SPEAKING QUESTIONS 1-2`  
Copy một cụm `{ ... }` và dán thêm vào danh sách:
```javascript
{
  id: 6, // Tăng số thứ tự
  title: "Đề Mới: Tên bài đọc",
  text: "Nội dung đoạn văn tiếng Anh ở đây...",
  vocab: [
    { word: "TừQuanTrọng", ipa: "/phiên-âm-ipa/" }
  ]
}
```

#### 2. Thêm bài viết Part 1 Writing (Viết theo tranh):
Tìm từ khóa: `// DATA: WRITING PART 1`  
Copy và dán thêm:
```javascript
{
  id: 11,
  icon: "🚗",
  context: "Mô tả bối cảnh tranh",
  hint: "Gợi ý ngữ pháp",
  words: "từ1 / từ2",
  userAnswer: "",
  showAnswer: false,
  modelAnswer: "Câu trả lời mẫu chuẩn.",
  advancedAnswer: "Câu nâng cao đạt điểm tuyệt đối."
}
```

#### 3. Thêm đề Email Part 2 Writing:
Tìm từ khóa: `// DATA: WRITING PART 2`  
Copy và dán thêm cấu trúc email tương tự.

### Bước 4: Lưu thay đổi (Commit)
- Cuộn xuống dưới cùng trang, bấm nút xanh lá cây **Commit changes**.
- Hệ thống GitHub Pages sẽ tự động kích hoạt và cập nhật lên web sau 30-60 giây!
