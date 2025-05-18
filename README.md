# 🇻🇳 Vietnamese ASR System - Automatic Speech Recognition

## 📚 Mô tả bài toán

Bài toán nhận diện tiếng nói tự động (ASR) cho tiếng Việt nhằm xây dựng một hệ thống có thể chuyển đổi âm thanh tiếng Việt thành văn bản với độ chính xác cao. Mục tiêu là giảm **Word Error Rate (WER)** thấp nhất có thể.

---

## 🧑‍💻 Phân chia công việc

| Thành viên       | MSSV       | Nhiệm vụ thực hiện                            |
|------------------|-------------|----------------------------------------------|
| Lê Thế Kỳ        | 20240837E   | Xử lý dữ liệu, tiền xử lý âm thanh           |
| Đỗ Đức Chiến     | 20240830E   | Huấn luyện mô hình, tối ưu hóa               |
| Tô Ánh Dương     | 20240822e   | Viết script đánh giá và tính WER             |
| Lưu Đăng Tuấn    | 20200557    | Trình bày slide báo cáo, viết README         |

---

## 🧠 Mô hình sử dụng

- ✅ Mô hình nền tảng: `Whiper` (Fine-tuned cho tiếng Việt)
- ✅ Thư viện: `torchaudio`, `transformers`, `pyctcdecode`,...
- ✅ Tăng cường dữ liệu: Thêm nhiễu nền, thay đổi tốc độ đọc

---

## 📁 Cấu trúc project

```bash
project/
│
├── dataset/                        # Dữ liệu âm thanh và transcript
│
│
├── src/
│   └── whisper-small-vi.ipynb
│
├── checkpoints/
│   └── README.md         
│
├── transcripts.txt             # Kết quả chuyển âm (dùng để chấm WER)
├── README.md                   # Tài liệu mô tả
├── slides.pdf                  #  Slide thuyết trình
└── report.docx                 # Báo cáo Word và
