# Gomoku 6×6 + ANN thay thế Heuristic cho Minimax

Đồ án được đóng gói trong **một file Jupyter Notebook duy nhất** nhằm thuận tiện cho việc chạy, kiểm thử và chấm điểm.

---

## 1. Yêu cầu hệ thống (Prerequisites)

Khuyến nghị sử dụng **Python 3.8 – 3.11**.

Cài đặt các thư viện cần thiết bằng lệnh:

```bash
pip install tensorflow numpy matplotlib scikit-learn
```

---

## 2. Hướng dẫn chạy chương trình

Toàn bộ mã nguồn nằm trong file:

```text
Gomoku_ANN_Minimax.ipynb
```

Bạn có thể mở và chạy notebook bằng một trong các công cụ sau:

- Visual Studio Code (kèm Jupyter Extension)
- Jupyter Notebook / JupyterLab
- Google Colab

### Các bước thực hiện

1. Mở file `Gomoku_ANN_Minimax.ipynb`.
2. Chạy (**Run**) các Cell **theo đúng thứ tự từ trên xuống dưới**.
3. **Không chạy bỏ qua Cell**, vì các Cell phía sau phụ thuộc vào biến, hàm và mô hình đã được khai báo ở các Cell trước.

> **Lưu ý:** Ở bước sinh dữ liệu (Cell 10) và quá trình huấn luyện mô hình ANN, chương trình có thể mất khoảng **20–60 giây** tùy theo cấu hình máy. Hãy chờ Cell chạy hoàn tất trước khi tiếp tục.

---

## 3. Lưu ý

### Kết quả thực nghiệm

- Đồ án đã thiết lập **random seed cố định** nhằm đảm bảo kết quả (Loss, Accuracy, ROC/AUC,...) được tái lập giữa các lần chạy.
- Điều này giúp việc kiểm thử và đối chiếu kết quả trong báo cáo được nhất quán.

### Giao diện Tkinter

Cell **9** sử dụng thư viện **Tkinter** để tạo giao diện cho phép người chơi đấu trực tiếp với AI Minimax.

- ✅ Hoạt động khi chạy trên **máy tính cá nhân (Local)**.
- ❌ **Không hoạt động trên Google Colab** do Colab không hỗ trợ hiển thị cửa sổ GUI.

Nếu chạy trên Google Colab, bạn có thể **bỏ qua Cell 9** và tiếp tục các Cell còn lại để xem quá trình huấn luyện, đánh giá mô hình và các biểu đồ kết quả.

---

## Cấu trúc dự án

```text
.
├── Gomoku_ANN_Minimax.ipynb   # Toàn bộ mã nguồn
├── gomoku_dataset.npz         # Dataset được sinh ra
├── [REPORT]_Gomoku_ANN.pdf    # Báo cáo
├── [PPTX]_Gomoku_ANN.pdf      # Slide thuyết trình
└── README.md
```
