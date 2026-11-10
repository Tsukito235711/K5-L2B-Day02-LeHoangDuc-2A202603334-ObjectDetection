# Báo cáo cá nhân — Ngày 2 Object Detection

Đổi tên file theo `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md`. Điền kết quả thật, xóa dòng hướng dẫn khi nộp. Xem [quy định nộp](../../SUBMISSION.md).

## 1. Thông tin học viên

- Họ tên: Le Hoang Duc
- MSSV: 2A2026003334
- Email: 26ai.duclh2@vinuni.edu.vn
- Lớp: L2
- Link repo bài làm:https://github.com/Tsukito235711/K5-L2B-Day02-LeHoangDuc-2A202603334-ObjectDetection
- Link Colab đã chạy:https://colab.research.google.com/drive/1ynJ3FaMsRY7EQtzqTvxsV4mhRM3Nv_c5#scrollTo=3e0508d8

## 2. Schema và mini guideline

Dẫn tới [GUIDELINE_MINI.md](../../GUIDELINE_MINI.md). Tóm tắt ba ca mơ hồ đã quyết định, cách áp dụng schema và phần cần giảng viên làm rõ.

## 3. Annotation và self-QC

- Số file nhãn train: 50
- Kết quả checker và lỗi đã xử lý: hop le
- Danh sách ít nhất 10 ảnh đã rà bằng mắt: 20-29
- Lỗi bỏ sót/box/class phát hiện khi rà và cách sửa: loi nhan chi bao nua so anh
- Commit khóa nhãn ban đầu:

## 4. Gold QC và rework

"iou_match_threshold": 0.5,
  "precision": 0.385,
  "recall": 0.7228,
  "f1": 0.5024,
  "mean_iou_of_matches": 0.8321,
  "true_positive": 472,
  "false_positive": 754,
  "false_negative": 181,
  "passed": false,
  "required_f1": 0.8,
  "required_mean_iou": 0.7
  FD va FN do file gold train index khac guide

| Chỉ số | Trước sửa | Sau sửa nếu có |
|---|---:|---:|
| TP | | |
| FP | | |
| FN | | |
| Precision | | |
| Recall | | |
| F1 | | |
| mean_iou_of_matches | | |
| passed | | |

Dẫn tới `outputs/annotation_evaluation.json` trong repo. Nếu rework, ghi ảnh, lỗi đã kiểm, quyết định sửa/giữ và lý do. Không suy nguyên nhân chỉ từ FP/FN. Không có rework thì ghi rõ.

## 5. Kết quả YOLO

- Runtime, GPU/CPU, phiên bản Ultralytics và Torch: python 3 cpu
- Các tham số thay đổi so với notebook nếu có và lý do: khong
- Đường dẫn best checkpoint trong phiên chạy: https://colab.research.google.com/drive/1ynJ3FaMsRY7EQtzqTvxsV4mhRM3Nv_c5#scrollTo=3e0508d8

| Chỉ số trên 10 ảnh eval | Giá trị |
|---|---:|
| Precision | 0.45904435300665103 |
| Recall | 0.24199967438957484 |
| mAP50 | 0.27467163992948657 |
| mAP50–95 | 0.2030939351794731 |

Đặt cả 2 folder `assets/eval_predictions/` và `assets/yolo26_runs/` (giải nén từ `day2_colab_outputs.zip`) cạnh báo cáo và dẫn link tương đối. Không chỉ ghi số; chỉ ra ít nhất một ảnh và vật thể cụ thể.

Trả lời bốn câu hỏi cuối notebook:

1. Lớp nào recall thấp nhất? Ảnh nào minh họa?
2. Nếu mAP50 cao nhưng mAP50–95 thấp, cần kiểm điều gì trên box?
3. Lỗi class nào có thể liên quan guideline? Dữ kiện nào hỗ trợ nhận xét?
4. Vì sao không dùng 10 ảnh eval để train? Vai trò validation của chúng trong notebook là gì?

## 6. Khó khăn và cách xử lý

| Bước/thời điểm | Lỗi quan sát | Cách đã thử | Kết quả/còn thiếu |
|---|---|---|---|
| | | | |

## 7. Tự đánh giá theo rubric

Đối chiếu [RUBRIC.md](../../RUBRIC.md): phần nào đã có kết quả, phần nào còn thiếu hoặc chưa kiểm được. Không tự nhận hoàn thành bước chưa chạy.

## 8. Công cụ AI và tài liệu tham khảo

Ghi công cụ đã dùng, dùng ở bước nào và phần đã tự kiểm tra; không dùng thì ghi rõ. Liệt kê nguồn ngoài repo được sử dụng. Không ghi mật khẩu/token hoặc đính kèm gold train.
