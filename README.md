# word_image_generator

## Chức năng: Sinh file Word từ ảnh gốc

## Yêu cầu
- Python 3 và pip
- File ảnh và file text để tạo ảnh

## Hướng dẫn sử dụng
1. Clone hoặc download repo này về máy bạn
2. Mở cmd/terminal và cd vào thư mục source code
3. Chạy `pip install -r requirements.txt`, nếu máy bạn có 2 bản Python thì là `pip3 install -r requirements.txt`
4. Đặt file ảnh và file text vào thư mục source code
5. Sửa 3 dòng sau (tất cả giá trị thay vào giữa cặp dấu ' '):
- image_path: Đường dẫn tới file ảnh
- text_path: Đường dẫn tới file text
- output_path: Đường dẫn tới file docx output
6. Chạy `python generate.py` nếu máy bạn có 2 bản Python thì là `python3 generate.py`

## Một số tham số có thể custom thêm
- Dòng 22, 23:
```python
section.page_width = Inches(16.54)
section.page_height = Inches(11.69)
```

Đây là kích cỡ rộng, dài, của khổ A4 ngang, nếu bạn tạo ảnh dọc thì có thể đổi kích cỡ thành A4 dọc:
```python
section.page_width = Inches(11.69)
section.page_height = Inches(16.54)
```
Ngoài ra bạn có thể custom 2 giá trị này thành các cỡ giấy khác nếu muốn, tuỳ theo bức ảnh của mình

- Dòng 25:
```python
styles.font.size = Pt(1.5)
```
Kích cỡ font chữ theo Pt

- Dòng 26:
```python
styles.font.name = 'Arial Black'
```

### Hãy Star nếu bạn thấy project này hữu ích <3
