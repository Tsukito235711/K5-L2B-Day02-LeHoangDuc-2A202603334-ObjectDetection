GUIDELINE_MINI

# Mini guideline — bài làm cá nhân

> Điền nội dung này trước khi bắt đầu gán nhãn. Giữ lại các quyết định sau khi self-QC.

## Định nghĩa lớp

| Lớp     | Định nghĩa của bạn | Ví dụ/điểm phân biệt  				    |
| ---     | ---                | ---                  				    |
| `car`   | Xe con 	       | Xe ô tô nhỏ 					    |
| `truck` | Xe tải             | Xe chở hàng hóa lớn, có thùng hàng 		    |
| `bus`   | Xe buýt            | Xe chở hành khách, kích thước hơi dài 		    |
| `van`   | Xe chở khách       | gần giống xe con nhưng dài hơn và ngắn hơn xe buýt |

## Quy tắc chung

- Box bám sát vật thể nghĩa là: cạnh box tiếp xúc với phần ngoài cùng của vật thể ở cả 4 phía, kích thước box nhỏ nhất có thể, không chứa bóng hay nền
- Vật thể bị che khuất: vẽ box cho toàn bộ phạm vi vật, kể cả phần bị che khuất nếu suy ra được hợp lí, nếu bị che hơn 80% thì bỏ qua
- Vật thể bị cắt bởi rìa ảnh: Vẽ box chỉ bao phần nhìn thấy trong ảnh, để cạnh box trùng với rìa ảnh, không vẽ ra ngoài khung hình.
- Vật thể rất nhỏ/mơ hồ: nếu không thể tự xác định chắc chắn thì không gán nhãn

## Ghi lại quyết định cho ít nhất ba ca mơ hồ

| Ảnh | Tình huống | Quyết định cuối | Lý do theo schema |
| --- | --- | --- | --- |
| `drive_001` | vật thể nhỏ và mờ| bỏ qua | không thể tự xác định chắc chắn |
| `drive_002` | vật thể bị che khuất hơn 80% | bỏ qua | vật thể bị che khuất hơn 80% |
| `drive_016` | mơ hồ giữa van và car | ghi chú lại hỏi | mơ hồ |
